# Comparing `tmp/mozmlops-0.0.2.tar.gz` & `tmp/mozmlops-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozmlops-0.0.2.tar", last modified: Mon Apr 29 22:35:24 2024, max compression
+gzip compressed data, was "mozmlops-0.1.1.tar", max compression
```

## Comparing `mozmlops-0.0.2.tar` & `mozmlops-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,10 @@
-drwxr-xr-x   0 chelseatroy   (501) staff       (20)        0 2024-04-29 22:35:24.320279 mozmlops-0.0.2/
--rw-r--r--   0 chelseatroy   (501) staff       (20)      434 2024-04-29 22:35:24.320032 mozmlops-0.0.2/PKG-INFO
-drwxr-xr-x   0 chelseatroy   (501) staff       (20)        0 2024-04-29 22:35:24.318724 mozmlops-0.0.2/mozmlops/
--rw-r--r--   0 chelseatroy   (501) staff       (20)        0 2024-04-29 22:35:10.000000 mozmlops-0.0.2/mozmlops/__init__.py
--rw-r--r--   0 chelseatroy   (501) staff       (20)     2162 2024-04-29 21:11:50.000000 mozmlops-0.0.2/mozmlops/artifact_store.py
-drwxr-xr-x   0 chelseatroy   (501) staff       (20)        0 2024-04-29 22:35:24.319605 mozmlops-0.0.2/mozmlops.egg-info/
--rw-r--r--   0 chelseatroy   (501) staff       (20)      434 2024-04-29 22:35:24.000000 mozmlops-0.0.2/mozmlops.egg-info/PKG-INFO
--rw-r--r--   0 chelseatroy   (501) staff       (20)      184 2024-04-29 22:35:24.000000 mozmlops-0.0.2/mozmlops.egg-info/SOURCES.txt
--rw-r--r--   0 chelseatroy   (501) staff       (20)        1 2024-04-29 22:35:24.000000 mozmlops-0.0.2/mozmlops.egg-info/dependency_links.txt
--rw-r--r--   0 chelseatroy   (501) staff       (20)        9 2024-04-29 22:35:24.000000 mozmlops-0.0.2/mozmlops.egg-info/top_level.txt
--rw-r--r--   0 chelseatroy   (501) staff       (20)       38 2024-04-29 22:35:24.320339 mozmlops-0.0.2/setup.cfg
--rw-r--r--   0 chelseatroy   (501) staff       (20)      806 2024-04-29 22:35:10.000000 mozmlops-0.0.2/setup.py
+-rwxr-xr-x   0        0        0    16726 2024-05-01 15:14:09.125008 mozmlops-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1914 2024-05-09 16:36:34.019400 mozmlops-0.1.1/README.md
+-rw-r--r--   0        0        0     1094 2024-05-22 07:36:52.356489 mozmlops-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-03 13:18:47.320679 mozmlops-0.1.1/src/mozmlops/.DS_Store
+-rw-r--r--   0        0        0      112 2024-05-22 07:36:29.548538 mozmlops-0.1.1/src/mozmlops/__init__.py
+-rw-r--r--   0        0        0     3714 2024-05-22 07:36:29.548853 mozmlops-0.1.1/src/mozmlops/cloud_storage_api_client.py
+-rw-r--r--   0        0        0     5131 2024-05-06 17:18:18.185607 mozmlops-0.1.1/src/mozmlops/templates/README.md
+-rw-r--r--   0        0        0       37 2024-05-06 17:18:18.185805 mozmlops-0.1.1/src/mozmlops/templates/example_config.json
+-rw-r--r--   0        0        0     4140 2024-05-22 07:36:29.549111 mozmlops-0.1.1/src/mozmlops/templates/template_flow.py
+-rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 mozmlops-0.1.1/PKG-INFO
```

