# Comparing `tmp/signaturesnet-0.0.4.tar.gz` & `tmp/signaturesnet-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signaturesnet-0.0.4.tar", last modified: Wed May 22 06:43:57 2024, max compression
+gzip compressed data, was "signaturesnet-0.0.5.tar", last modified: Wed May 22 06:55:41 2024, max compression
```

## Comparing `signaturesnet-0.0.4.tar` & `signaturesnet-0.0.5.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.627665 signaturesnet-0.0.4/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1064 2024-05-08 20:34:21.000000 signaturesnet-0.0.4/LICENSE
--rw-r--r--   0 oleguer   (1000) oleguer   (1000)     6876 2024-05-22 06:43:57.627665 signaturesnet-0.0.4/PKG-INFO
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     6323 2024-05-17 07:24:47.000000 signaturesnet-0.0.4/README.md
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)       38 2024-05-22 06:43:57.627665 signaturesnet-0.0.4/setup.cfg
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      863 2024-05-22 06:42:12.000000 signaturesnet-0.0.4/setup.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.623665 signaturesnet-0.0.4/signaturesnet/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      197 2024-05-22 06:34:54.000000 signaturesnet-0.0.4/signaturesnet/__init__.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.623665 signaturesnet-0.0.4/signaturesnet/loggers/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      189 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/loggers/__init__.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1036 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/loggers/classifier_logger.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      668 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/loggers/errorfinder_logger.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1689 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/loggers/finetuner_logger.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     4566 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/loggers/generator_logger.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      600 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/loggers/nummut_logger.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.623665 signaturesnet-0.0.4/signaturesnet/models/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      229 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/models/__init__.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3269 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/models/baseline.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2102 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/models/classifier.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     4185 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/models/errorfinder.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     8037 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/models/finetuner.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5396 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/models/generator.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1963 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/models/nummut.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.623665 signaturesnet-0.0.4/signaturesnet/modules/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      118 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/modules/__init__.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5444 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/modules/classified_tunning_error.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3164 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/modules/combined_finetuner.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9606 2024-05-22 06:35:53.000000 signaturesnet-0.0.4/signaturesnet/modules/signet_module.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1936 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/train_classifier.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3421 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/train_errorfinder.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2559 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/train_finetuner.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3030 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/train_generator.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1673 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/train_nummutnet.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.623665 signaturesnet-0.0.4/signaturesnet/trainers/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      315 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/trainers/__init__.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5607 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/trainers/classifier_trainer.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)    13270 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/trainers/error_trainer.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5319 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/trainers/finetuner_crossvalidation.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9103 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/trainers/finetuner_trainer.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9620 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/trainers/generator_trainer.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5714 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/trainers/nummut_trainer.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.627665 signaturesnet-0.0.4/signaturesnet/utilities/
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     7006 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/utilities/VCF_to_counts.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:33:09.000000 signaturesnet-0.0.4/signaturesnet/utilities/__init__.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     7332 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/utilities/data_generator.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2949 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/utilities/data_partitions.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      460 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/utilities/generator_data.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      924 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/utilities/helpers.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)    17699 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/utilities/io.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)    13895 2024-05-08 20:34:22.000000 signaturesnet-0.0.4/signaturesnet/utilities/metrics.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2549 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/utilities/normalize_data.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5342 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/utilities/oversampler.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)    47058 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/utilities/plotting.py
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     4898 2024-05-15 17:24:40.000000 signaturesnet-0.0.4/signaturesnet/utilities/temporal_io.py
-drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:43:57.627665 signaturesnet-0.0.4/signaturesnet.egg-info/
--rw-r--r--   0 oleguer   (1000) oleguer   (1000)     6876 2024-05-22 06:43:57.000000 signaturesnet-0.0.4/signaturesnet.egg-info/PKG-INFO
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1812 2024-05-22 06:43:57.000000 signaturesnet-0.0.4/signaturesnet.egg-info/SOURCES.txt
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)        1 2024-05-22 06:43:57.000000 signaturesnet-0.0.4/signaturesnet.egg-info/dependency_links.txt
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      122 2024-05-22 06:43:57.000000 signaturesnet-0.0.4/signaturesnet.egg-info/requires.txt
--rw-rw-r--   0 oleguer   (1000) oleguer   (1000)       14 2024-05-22 06:43:57.000000 signaturesnet-0.0.4/signaturesnet.egg-info/top_level.txt
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:55:41.544333 signaturesnet-0.0.5/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1064 2024-05-08 20:34:21.000000 signaturesnet-0.0.5/LICENSE
+-rw-r--r--   0 oleguer   (1000) oleguer   (1000)     6889 2024-05-22 06:55:41.544333 signaturesnet-0.0.5/PKG-INFO
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     6336 2024-05-22 06:46:41.000000 signaturesnet-0.0.5/README.md
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)       38 2024-05-22 06:55:41.544333 signaturesnet-0.0.5/setup.cfg
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      863 2024-05-22 06:47:40.000000 signaturesnet-0.0.5/setup.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:55:41.540333 signaturesnet-0.0.5/signaturesnet/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      197 2024-05-22 06:47:21.000000 signaturesnet-0.0.5/signaturesnet/__init__.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:55:41.540333 signaturesnet-0.0.5/signaturesnet/data/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:51:15.000000 signaturesnet-0.0.5/signaturesnet/data/__init__.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:55:41.540333 signaturesnet-0.0.5/signaturesnet/loggers/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      189 2024-05-08 20:34:22.000000 signaturesnet-0.0.5/signaturesnet/loggers/__init__.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1036 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/loggers/classifier_logger.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      668 2024-05-08 20:34:22.000000 signaturesnet-0.0.5/signaturesnet/loggers/errorfinder_logger.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1689 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/loggers/finetuner_logger.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     4566 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/loggers/generator_logger.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      600 2024-05-08 20:34:22.000000 signaturesnet-0.0.5/signaturesnet/loggers/nummut_logger.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:55:41.540333 signaturesnet-0.0.5/signaturesnet/models/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      229 2024-05-08 20:34:22.000000 signaturesnet-0.0.5/signaturesnet/models/__init__.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3269 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/models/baseline.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2102 2024-05-08 20:34:22.000000 signaturesnet-0.0.5/signaturesnet/models/classifier.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     4185 2024-05-08 20:34:22.000000 signaturesnet-0.0.5/signaturesnet/models/errorfinder.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     8037 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/models/finetuner.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5396 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/models/generator.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1963 2024-05-08 20:34:22.000000 signaturesnet-0.0.5/signaturesnet/models/nummut.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:55:41.540333 signaturesnet-0.0.5/signaturesnet/modules/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      118 2024-05-08 20:34:22.000000 signaturesnet-0.0.5/signaturesnet/modules/__init__.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5444 2024-05-08 20:34:22.000000 signaturesnet-0.0.5/signaturesnet/modules/classified_tunning_error.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3164 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/modules/combined_finetuner.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9606 2024-05-22 06:35:53.000000 signaturesnet-0.0.5/signaturesnet/modules/signet_module.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1936 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/train_classifier.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3421 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/train_errorfinder.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2559 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/train_finetuner.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     3030 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/train_generator.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1673 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/train_nummutnet.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:55:41.540333 signaturesnet-0.0.5/signaturesnet/trainers/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      315 2024-05-08 20:34:22.000000 signaturesnet-0.0.5/signaturesnet/trainers/__init__.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5607 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/trainers/classifier_trainer.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)    13270 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/trainers/error_trainer.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5319 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/trainers/finetuner_crossvalidation.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9103 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/trainers/finetuner_trainer.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     9620 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/trainers/generator_trainer.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5714 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/trainers/nummut_trainer.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:55:41.544333 signaturesnet-0.0.5/signaturesnet/utilities/
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     7006 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/utilities/VCF_to_counts.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:33:09.000000 signaturesnet-0.0.5/signaturesnet/utilities/__init__.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     7332 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/utilities/data_generator.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2949 2024-05-08 20:34:22.000000 signaturesnet-0.0.5/signaturesnet/utilities/data_partitions.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      460 2024-05-08 20:34:22.000000 signaturesnet-0.0.5/signaturesnet/utilities/generator_data.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      924 2024-05-08 20:34:22.000000 signaturesnet-0.0.5/signaturesnet/utilities/helpers.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)    17699 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/utilities/io.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)    13895 2024-05-08 20:34:22.000000 signaturesnet-0.0.5/signaturesnet/utilities/metrics.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     2549 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/utilities/normalize_data.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     5342 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/utilities/oversampler.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)    47058 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/utilities/plotting.py
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     4898 2024-05-15 17:24:40.000000 signaturesnet-0.0.5/signaturesnet/utilities/temporal_io.py
+drwxrwxr-x   0 oleguer   (1000) oleguer   (1000)        0 2024-05-22 06:55:41.544333 signaturesnet-0.0.5/signaturesnet.egg-info/
+-rw-r--r--   0 oleguer   (1000) oleguer   (1000)     6889 2024-05-22 06:55:41.000000 signaturesnet-0.0.5/signaturesnet.egg-info/PKG-INFO
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)     1843 2024-05-22 06:55:41.000000 signaturesnet-0.0.5/signaturesnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)        1 2024-05-22 06:55:41.000000 signaturesnet-0.0.5/signaturesnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)      122 2024-05-22 06:55:41.000000 signaturesnet-0.0.5/signaturesnet.egg-info/requires.txt
+-rw-rw-r--   0 oleguer   (1000) oleguer   (1000)       14 2024-05-22 06:55:41.000000 signaturesnet-0.0.5/signaturesnet.egg-info/top_level.txt
```

### Comparing `signaturesnet-0.0.4/LICENSE` & `signaturesnet-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/PKG-INFO` & `signaturesnet-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signaturesnet
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package to manipulate mutational processes.
 Home-page: https://github.com/weghornlab/SigNet
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: scipy
 Requires-Dist: numpy
@@ -57,22 +57,22 @@
 pip install signaturesnet
 ```
 
 Once installed, you can run Signet Refitter like so:
 
 ```python
 import pandas as pd
-import signaturesnet
+from signaturesnet.modules.signet_module import SigNet
 
 # Read your mutational data
 mutations = pd.read_csv("your_input", header=0, index_col=0)
 
-# Load & Run signaturesnet
-signaturesnet = SigNet(opportunities_name_or_path="your_normalization_file")
-results = signaturesnet(mutation_dataset=mutations)
+# Load & Run signet
+signet = SigNet(opportunities_name_or_path="your_normalization_file")
+results = signet(mutation_dataset=mutations)
 
 # Extract results
 w, u, l, c, _ = results.get_output()
 
 # Store results
 results.save(path='Output', name="this_experiment_filename")
```

### Comparing `signaturesnet-0.0.4/README.md` & `signaturesnet-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,22 @@
 pip install signaturesnet
 ```
 
 Once installed, you can run Signet Refitter like so:
 
 ```python
 import pandas as pd
-import signaturesnet
+from signaturesnet.modules.signet_module import SigNet
 
 # Read your mutational data
 mutations = pd.read_csv("your_input", header=0, index_col=0)
 
-# Load & Run signaturesnet
-signaturesnet = SigNet(opportunities_name_or_path="your_normalization_file")
-results = signaturesnet(mutation_dataset=mutations)
+# Load & Run signet
+signet = SigNet(opportunities_name_or_path="your_normalization_file")
+results = signet(mutation_dataset=mutations)
 
 # Extract results
 w, u, l, c, _ = results.get_output()
 
 # Store results
 results.save(path='Output', name="this_experiment_filename")
```

### Comparing `signaturesnet-0.0.4/setup.py` & `signaturesnet-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Read the content of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='signaturesnet',
-      version='0.0.4',
+      version='0.0.5',
       description="Package to manipulate mutational processes.",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/weghornlab/SigNet',
       packages=find_packages(),
       install_requires=[
             'torch',
```

### Comparing `signaturesnet-0.0.4/signaturesnet/loggers/classifier_logger.py` & `signaturesnet-0.0.5/signaturesnet/loggers/classifier_logger.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/loggers/errorfinder_logger.py` & `signaturesnet-0.0.5/signaturesnet/loggers/errorfinder_logger.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/loggers/finetuner_logger.py` & `signaturesnet-0.0.5/signaturesnet/loggers/finetuner_logger.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/loggers/generator_logger.py` & `signaturesnet-0.0.5/signaturesnet/loggers/generator_logger.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/loggers/nummut_logger.py` & `signaturesnet-0.0.5/signaturesnet/loggers/nummut_logger.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/models/baseline.py` & `signaturesnet-0.0.5/signaturesnet/models/baseline.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/models/classifier.py` & `signaturesnet-0.0.5/signaturesnet/models/classifier.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/models/errorfinder.py` & `signaturesnet-0.0.5/signaturesnet/models/errorfinder.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/models/finetuner.py` & `signaturesnet-0.0.5/signaturesnet/models/finetuner.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/models/generator.py` & `signaturesnet-0.0.5/signaturesnet/models/generator.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/models/nummut.py` & `signaturesnet-0.0.5/signaturesnet/models/nummut.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/modules/classified_tunning_error.py` & `signaturesnet-0.0.5/signaturesnet/modules/classified_tunning_error.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/modules/combined_finetuner.py` & `signaturesnet-0.0.5/signaturesnet/modules/combined_finetuner.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/modules/signet_module.py` & `signaturesnet-0.0.5/signaturesnet/modules/signet_module.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/train_classifier.py` & `signaturesnet-0.0.5/signaturesnet/train_classifier.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/train_errorfinder.py` & `signaturesnet-0.0.5/signaturesnet/train_errorfinder.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/train_finetuner.py` & `signaturesnet-0.0.5/signaturesnet/train_finetuner.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/train_generator.py` & `signaturesnet-0.0.5/signaturesnet/train_generator.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/train_nummutnet.py` & `signaturesnet-0.0.5/signaturesnet/train_nummutnet.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/trainers/classifier_trainer.py` & `signaturesnet-0.0.5/signaturesnet/trainers/classifier_trainer.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/trainers/error_trainer.py` & `signaturesnet-0.0.5/signaturesnet/trainers/error_trainer.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/trainers/finetuner_crossvalidation.py` & `signaturesnet-0.0.5/signaturesnet/trainers/finetuner_crossvalidation.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/trainers/finetuner_trainer.py` & `signaturesnet-0.0.5/signaturesnet/trainers/finetuner_trainer.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/trainers/generator_trainer.py` & `signaturesnet-0.0.5/signaturesnet/trainers/generator_trainer.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/trainers/nummut_trainer.py` & `signaturesnet-0.0.5/signaturesnet/trainers/nummut_trainer.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/utilities/VCF_to_counts.py` & `signaturesnet-0.0.5/signaturesnet/utilities/VCF_to_counts.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/utilities/data_generator.py` & `signaturesnet-0.0.5/signaturesnet/utilities/data_generator.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/utilities/data_partitions.py` & `signaturesnet-0.0.5/signaturesnet/utilities/data_partitions.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/utilities/helpers.py` & `signaturesnet-0.0.5/signaturesnet/utilities/helpers.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/utilities/io.py` & `signaturesnet-0.0.5/signaturesnet/utilities/io.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/utilities/metrics.py` & `signaturesnet-0.0.5/signaturesnet/utilities/metrics.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/utilities/normalize_data.py` & `signaturesnet-0.0.5/signaturesnet/utilities/normalize_data.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/utilities/oversampler.py` & `signaturesnet-0.0.5/signaturesnet/utilities/oversampler.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/utilities/plotting.py` & `signaturesnet-0.0.5/signaturesnet/utilities/plotting.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet/utilities/temporal_io.py` & `signaturesnet-0.0.5/signaturesnet/utilities/temporal_io.py`

 * *Files identical despite different names*

### Comparing `signaturesnet-0.0.4/signaturesnet.egg-info/PKG-INFO` & `signaturesnet-0.0.5/signaturesnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signaturesnet
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package to manipulate mutational processes.
 Home-page: https://github.com/weghornlab/SigNet
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: scipy
 Requires-Dist: numpy
@@ -57,22 +57,22 @@
 pip install signaturesnet
 ```
 
 Once installed, you can run Signet Refitter like so:
 
 ```python
 import pandas as pd
-import signaturesnet
+from signaturesnet.modules.signet_module import SigNet
 
 # Read your mutational data
 mutations = pd.read_csv("your_input", header=0, index_col=0)
 
-# Load & Run signaturesnet
-signaturesnet = SigNet(opportunities_name_or_path="your_normalization_file")
-results = signaturesnet(mutation_dataset=mutations)
+# Load & Run signet
+signet = SigNet(opportunities_name_or_path="your_normalization_file")
+results = signet(mutation_dataset=mutations)
 
 # Extract results
 w, u, l, c, _ = results.get_output()
 
 # Store results
 results.save(path='Output', name="this_experiment_filename")
```

### Comparing `signaturesnet-0.0.4/signaturesnet.egg-info/SOURCES.txt` & `signaturesnet-0.0.5/signaturesnet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 signaturesnet/train_generator.py
 signaturesnet/train_nummutnet.py
 signaturesnet.egg-info/PKG-INFO
 signaturesnet.egg-info/SOURCES.txt
 signaturesnet.egg-info/dependency_links.txt
 signaturesnet.egg-info/requires.txt
 signaturesnet.egg-info/top_level.txt
+signaturesnet/data/__init__.py
 signaturesnet/loggers/__init__.py
 signaturesnet/loggers/classifier_logger.py
 signaturesnet/loggers/errorfinder_logger.py
 signaturesnet/loggers/finetuner_logger.py
 signaturesnet/loggers/generator_logger.py
 signaturesnet/loggers/nummut_logger.py
 signaturesnet/models/__init__.py
```

