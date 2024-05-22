# Comparing `tmp/signaturesnet-0.0.3.tar.gz` & `tmp/signaturesnet-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signaturesnet-0.0.3.tar", last modified: Sun May 19 17:10:04 2024, max compression
+gzip compressed data, was "signaturesnet-0.0.4.tar", last modified: Wed May 22 06:43:57 2024, max compression
```

## Comparing `signaturesnet-0.0.3.tar` & `signaturesnet-0.0.4.tar`

### file list

```diff
@@ -1,47 +1,60 @@
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-19 17:10:04.871119 signaturesnet-0.0.3/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1064 2024-05-08 20:34:21.000000 signaturesnet-0.0.3/LICENSE
--rw-r--r--   0 oleguer   (1000) oleguer   (1000)     6876 2024-05-19 17:10:04.871119 signaturesnet-0.0.3/PKG-INFO
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     6323 2024-05-17 07:24:47.000000 signaturesnet-0.0.3/README.md
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)       38 2024-05-19 17:10:04.871119 signaturesnet-0.0.3/setup.cfg
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      863 2024-05-19 17:06:27.000000 signaturesnet-0.0.3/setup.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-19 17:10:04.863119 signaturesnet-0.0.3/signaturesnet/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      197 2024-05-08 20:34:21.000000 signaturesnet-0.0.3/signaturesnet/__init__.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-19 17:10:04.867118 signaturesnet-0.0.3/signaturesnet/loggers/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      189 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/loggers/__init__.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1036 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/loggers/classifier_logger.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      668 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/loggers/errorfinder_logger.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1689 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/loggers/finetuner_logger.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     4566 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/loggers/generator_logger.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      600 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/loggers/nummut_logger.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-19 17:10:04.867118 signaturesnet-0.0.3/signaturesnet/models/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      229 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/models/__init__.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3269 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/models/baseline.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2102 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/models/classifier.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     4185 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/models/errorfinder.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     8037 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/models/finetuner.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5396 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/models/generator.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1963 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/models/nummut.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-19 17:10:04.871119 signaturesnet-0.0.3/signaturesnet/modules/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      118 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/modules/__init__.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5444 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/modules/classified_tunning_error.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3164 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/modules/combined_finetuner.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9604 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/modules/signet_module.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1936 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/train_classifier.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3421 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/train_errorfinder.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2559 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/train_finetuner.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3030 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/train_generator.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1673 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/train_nummutnet.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-19 17:10:04.871119 signaturesnet-0.0.3/signaturesnet/trainers/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      315 2024-05-08 20:34:22.000000 signaturesnet-0.0.3/signaturesnet/trainers/__init__.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5607 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/trainers/classifier_trainer.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)    13270 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/trainers/error_trainer.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5319 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/trainers/finetuner_crossvalidation.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9103 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/trainers/finetuner_trainer.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9620 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/trainers/generator_trainer.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5714 2024-05-15 17:24:40.000000 signaturesnet-0.0.3/signaturesnet/trainers/nummut_trainer.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-19 17:10:04.871119 signaturesnet-0.0.3/signaturesnet.egg-info/
--rw-r--r--   0 oleguer   (1000) oleguer   (1000)     6876 2024-05-19 17:10:04.000000 signaturesnet-0.0.3/signaturesnet.egg-info/PKG-INFO
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1352 2024-05-19 17:10:04.000000 signaturesnet-0.0.3/signaturesnet.egg-info/SOURCES.txt
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)        1 2024-05-19 17:10:04.000000 signaturesnet-0.0.3/signaturesnet.egg-info/dependency_links.txt
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      122 2024-05-19 17:10:04.000000 signaturesnet-0.0.3/signaturesnet.egg-info/requires.txt
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)       14 2024-05-19 17:10:04.000000 signaturesnet-0.0.3/signaturesnet.egg-info/top_level.txt
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.627665 signaturesnet-0.0.4/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1064 2024-05-08 20:34:21.000000 signaturesnet-0.0.4/LICENSE
+-rw-r--r--   0 oleguer   (1000) oleguer   (1000)     6876 2024-05-22 06:43:57.627665 signaturesnet-0.0.4/PKG-INFO
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     6323 2024-05-17 07:24:47.000000 signaturesnet-0.0.4/README.md
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)       38 2024-05-22 06:43:57.627665 signaturesnet-0.0.4/setup.cfg
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      863 2024-05-22 06:42:12.000000 signaturesnet-0.0.4/setup.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.623665 signaturesnet-0.0.4/signaturesnet/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      197 2024-05-22 06:34:54.000000 signaturesnet-0.0.4/signaturesnet/__init__.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.623665 signaturesnet-0.0.4/signaturesnet/loggers/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      189 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/loggers/__init__.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1036 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/loggers/classifier_logger.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      668 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/loggers/errorfinder_logger.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1689 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/loggers/finetuner_logger.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     4566 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/loggers/generator_logger.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      600 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/loggers/nummut_logger.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.623665 signaturesnet-0.0.4/signaturesnet/models/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      229 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/models/__init__.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3269 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/models/baseline.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2102 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/models/classifier.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     4185 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/models/errorfinder.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     8037 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/models/finetuner.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5396 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/models/generator.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1963 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/models/nummut.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.623665 signaturesnet-0.0.4/signaturesnet/modules/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      118 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/modules/__init__.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5444 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/modules/classified_tunning_error.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3164 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/modules/combined_finetuner.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9606 2024-05-22 06:35:53.000000 signaturesnet-0.0.4/signaturesnet/modules/signet_module.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1936 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/train_classifier.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3421 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/train_errorfinder.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2559 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/train_finetuner.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3030 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/train_generator.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1673 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/train_nummutnet.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.623665 signaturesnet-0.0.4/signaturesnet/trainers/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      315 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/trainers/__init__.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5607 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/trainers/classifier_trainer.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)    13270 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/trainers/error_trainer.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5319 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/trainers/finetuner_crossvalidation.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9103 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/trainers/finetuner_trainer.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9620 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/trainers/generator_trainer.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5714 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/trainers/nummut_trainer.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.627665 signaturesnet-0.0.4/signaturesnet/utilities/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     7006 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/utilities/VCF_to_counts.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:33:09.000000 signaturesnet-0.0.4/signaturesnet/utilities/__init__.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     7332 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/utilities/data_generator.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2949 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/utilities/data_partitions.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      460 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/utilities/generator_data.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      924 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/utilities/helpers.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)    17699 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/utilities/io.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)    13895 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/utilities/metrics.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2549 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/utilities/normalize_data.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5342 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/utilities/oversampler.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)    47058 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/utilities/plotting.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     4898 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/utilities/temporal_io.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.627665 signaturesnet-0.0.4/signaturesnet.egg-info/
+-rw-r--r--   0 oleguer   (1000) oleguer   (1000)     6876 2024-05-22 06:43:57.000000 signaturesnet-0.0.4/signaturesnet.egg-info/PKG-INFO
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1812 2024-05-22 06:43:57.000000 signaturesnet-0.0.4/signaturesnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)        1 2024-05-22 06:43:57.000000 signaturesnet-0.0.4/signaturesnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      122 2024-05-22 06:43:57.000000 signaturesnet-0.0.4/signaturesnet.egg-info/requires.txt
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)       14 2024-05-22 06:43:57.000000 signaturesnet-0.0.4/signaturesnet.egg-info/top_level.txt
```

### Comparing `signaturesnet-0.0.3/LICENSE` & `signaturesnet-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/PKG-INFO` & `signaturesnet-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signaturesnet
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package to manipulate mutational processes.
 Home-page: https://github.com/weghornlab/SigNet
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: scipy
 Requires-Dist: numpy
```

### Comparing `signaturesnet-0.0.3/README.md` & `signaturesnet-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/setup.py` & `signaturesnet-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Read the content of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='signaturesnet',
-      version='0.0.3',
+      version='0.0.4',
       description="Package to manipulate mutational processes.",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/weghornlab/SigNet',
       packages=find_packages(),
       install_requires=[
             'torch',
```

### Comparing `signaturesnet-0.0.3/signaturesnet/loggers/classifier_logger.py` & `signaturesnet-0.0.4/signaturesnet/loggers/classifier_logger.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/loggers/errorfinder_logger.py` & `signaturesnet-0.0.4/signaturesnet/loggers/errorfinder_logger.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/loggers/finetuner_logger.py` & `signaturesnet-0.0.4/signaturesnet/loggers/finetuner_logger.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/loggers/generator_logger.py` & `signaturesnet-0.0.4/signaturesnet/loggers/generator_logger.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/loggers/nummut_logger.py` & `signaturesnet-0.0.4/signaturesnet/loggers/nummut_logger.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/models/baseline.py` & `signaturesnet-0.0.4/signaturesnet/models/baseline.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/models/classifier.py` & `signaturesnet-0.0.4/signaturesnet/models/classifier.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/models/errorfinder.py` & `signaturesnet-0.0.4/signaturesnet/models/errorfinder.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/models/finetuner.py` & `signaturesnet-0.0.4/signaturesnet/models/finetuner.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/models/generator.py` & `signaturesnet-0.0.4/signaturesnet/models/generator.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/models/nummut.py` & `signaturesnet-0.0.4/signaturesnet/models/nummut.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/modules/classified_tunning_error.py` & `signaturesnet-0.0.4/signaturesnet/modules/classified_tunning_error.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/modules/combined_finetuner.py` & `signaturesnet-0.0.4/signaturesnet/modules/combined_finetuner.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/modules/signet_module.py` & `signaturesnet-0.0.4/signaturesnet/modules/signet_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         """
         with torch.no_grad():
             # Sort input data columns
             mutation_order = pd.read_excel(os.path.join(DATA, "mutation_type_order.xlsx"))
             mutation_dataset = mutation_dataset[list(mutation_order['Type'])]
             sample_names = mutation_dataset.index
 
-            mutation_vec = torch.tensor(mutation_dataset.values.astype(np.float), dtype=torch.float, device='cpu')
+            mutation_vec = torch.tensor(mutation_dataset.values.astype(np.float32), dtype=torch.float, device='cpu')
             num_mutations = torch.sum(mutation_vec, dim=1)
 
             # Normalize input data
             if self.opportunities_name_or_path is not None:
                 mutation_vec = normalize_data(mutation_vec, self.opportunities_name_or_path)
 
             sums = torch.sum(mutation_vec, dim=1).reshape(-1, 1)
```

### Comparing `signaturesnet-0.0.3/signaturesnet/train_classifier.py` & `signaturesnet-0.0.4/signaturesnet/train_classifier.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/train_errorfinder.py` & `signaturesnet-0.0.4/signaturesnet/train_errorfinder.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/train_finetuner.py` & `signaturesnet-0.0.4/signaturesnet/train_finetuner.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/train_generator.py` & `signaturesnet-0.0.4/signaturesnet/train_generator.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/train_nummutnet.py` & `signaturesnet-0.0.4/signaturesnet/train_nummutnet.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/trainers/classifier_trainer.py` & `signaturesnet-0.0.4/signaturesnet/trainers/classifier_trainer.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/trainers/error_trainer.py` & `signaturesnet-0.0.4/signaturesnet/trainers/error_trainer.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/trainers/finetuner_crossvalidation.py` & `signaturesnet-0.0.4/signaturesnet/trainers/finetuner_crossvalidation.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/trainers/finetuner_trainer.py` & `signaturesnet-0.0.4/signaturesnet/trainers/finetuner_trainer.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/trainers/generator_trainer.py` & `signaturesnet-0.0.4/signaturesnet/trainers/generator_trainer.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet/trainers/nummut_trainer.py` & `signaturesnet-0.0.4/signaturesnet/trainers/nummut_trainer.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.3/signaturesnet.egg-info/PKG-INFO` & `signaturesnet-0.0.4/signaturesnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signaturesnet
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package to manipulate mutational processes.
 Home-page: https://github.com/weghornlab/SigNet
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: scipy
 Requires-Dist: numpy
```

### Comparing `signaturesnet-0.0.3/signaturesnet.egg-info/SOURCES.txt` & `signaturesnet-0.0.4/signaturesnet.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -31,8 +31,20 @@
 signaturesnet/modules/signet_module.py
 signaturesnet/trainers/__init__.py
 signaturesnet/trainers/classifier_trainer.py
 signaturesnet/trainers/error_trainer.py
 signaturesnet/trainers/finetuner_crossvalidation.py
 signaturesnet/trainers/finetuner_trainer.py
 signaturesnet/trainers/generator_trainer.py
-signaturesnet/trainers/nummut_trainer.py
+signaturesnet/trainers/nummut_trainer.py
+signaturesnet/utilities/VCF_to_counts.py
+signaturesnet/utilities/__init__.py
+signaturesnet/utilities/data_generator.py
+signaturesnet/utilities/data_partitions.py
+signaturesnet/utilities/generator_data.py
+signaturesnet/utilities/helpers.py
+signaturesnet/utilities/io.py
+signaturesnet/utilities/metrics.py
+signaturesnet/utilities/normalize_data.py
+signaturesnet/utilities/oversampler.py
+signaturesnet/utilities/plotting.py
+signaturesnet/utilities/temporal_io.py
```

