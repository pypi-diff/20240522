# Comparing `tmp/clockwise-1.0.0.tar.gz` & `tmp/clockwise-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clockwise-1.0.0.tar", last modified: Thu Nov  9 09:15:34 2023, max compression
+gzip compressed data, was "clockwise-1.0.1.tar", last modified: Wed May 22 17:36:23 2024, max compression
```

## Comparing `clockwise-1.0.0.tar` & `clockwise-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 sele       (501) staff       (20)        0 2023-11-09 09:15:34.696812 clockwise-1.0.0/
--rw-r--r--   0 sele       (501) staff       (20)     1070 2023-09-24 18:07:04.000000 clockwise-1.0.0/LICENSE
--rw-r--r--   0 sele       (501) staff       (20)      930 2023-11-09 09:15:34.696278 clockwise-1.0.0/PKG-INFO
--rw-r--r--   0 sele       (501) staff       (20)      342 2023-11-09 08:49:30.000000 clockwise-1.0.0/README.md
-drwxr-xr-x   0 sele       (501) staff       (20)        0 2023-11-09 09:15:34.695728 clockwise-1.0.0/clockwise.egg-info/
--rw-r--r--   0 sele       (501) staff       (20)      930 2023-11-09 09:15:34.000000 clockwise-1.0.0/clockwise.egg-info/PKG-INFO
--rw-r--r--   0 sele       (501) staff       (20)      205 2023-11-09 09:15:34.000000 clockwise-1.0.0/clockwise.egg-info/SOURCES.txt
--rw-r--r--   0 sele       (501) staff       (20)        1 2023-11-09 09:15:34.000000 clockwise-1.0.0/clockwise.egg-info/dependency_links.txt
--rw-r--r--   0 sele       (501) staff       (20)        7 2023-11-09 09:15:34.000000 clockwise-1.0.0/clockwise.egg-info/requires.txt
--rw-r--r--   0 sele       (501) staff       (20)        1 2023-11-09 09:15:34.000000 clockwise-1.0.0/clockwise.egg-info/top_level.txt
--rw-r--r--   0 sele       (501) staff       (20)      528 2023-11-09 09:13:36.000000 clockwise-1.0.0/pyproject.toml
--rw-r--r--   0 sele       (501) staff       (20)       38 2023-11-09 09:15:34.696910 clockwise-1.0.0/setup.cfg
--rw-r--r--   0 sele       (501) staff       (20)      341 2023-11-09 08:54:54.000000 clockwise-1.0.0/setup.py
+drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2024-05-22 17:36:23.688257 clockwise-1.0.1/
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     1070 2024-05-22 11:14:20.000000 clockwise-1.0.1/LICENSE
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      207 2024-05-22 17:36:23.688257 clockwise-1.0.1/PKG-INFO
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      342 2024-05-22 11:14:20.000000 clockwise-1.0.1/README.md
+drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2024-05-22 17:36:23.672257 clockwise-1.0.1/clockwise/
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      230 2024-05-22 17:36:19.000000 clockwise-1.0.1/clockwise/__init__.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     2768 2024-05-22 17:31:23.000000 clockwise-1.0.1/clockwise/clockwise.py
+drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2024-05-22 17:36:23.684257 clockwise-1.0.1/clockwise.egg-info/
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      207 2024-05-22 17:36:23.000000 clockwise-1.0.1/clockwise.egg-info/PKG-INFO
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      213 2024-05-22 17:36:23.000000 clockwise-1.0.1/clockwise.egg-info/SOURCES.txt
+-rw-r--r--   0 sas      (23222) tumuser  (20909)        1 2024-05-22 17:36:23.000000 clockwise-1.0.1/clockwise.egg-info/dependency_links.txt
+-rw-r--r--   0 sas      (23222) tumuser  (20909)       10 2024-05-22 17:36:23.000000 clockwise-1.0.1/clockwise.egg-info/top_level.txt
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      103 2024-05-22 17:36:23.688257 clockwise-1.0.1/setup.cfg
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      287 2024-05-22 17:36:11.000000 clockwise-1.0.1/setup.py
```

### Comparing `clockwise-1.0.0/LICENSE` & `clockwise-1.0.1/LICENSE`

 * *Files identical despite different names*

