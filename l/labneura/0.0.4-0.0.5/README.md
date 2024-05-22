# Comparing `tmp/labneura-0.0.4.tar.gz` & `tmp/labneura-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "labneura-0.0.5.tar", last modified: Wed May 22 16:53:07 2024, max compression
```

## Comparing `labneura-0.0.4.tar` & `labneura-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,14 @@
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 labneura-0.0.4/Makefile
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 labneura-0.0.4/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 labneura-0.0.4/requirements.txt
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 labneura-0.0.4/src/__init__.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 labneura-0.0.4/src/labneura/__init__.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 labneura-0.0.4/src/labneura/eda/__init__.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 labneura-0.0.4/src/labneura/eda/checker.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 labneura-0.0.4/src/labneura/eda/profiler.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 labneura-0.0.4/src/labneura/eda/reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labneura-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 labneura-0.0.4/tests/test_profiler.py
--rw-r--r--   0        0        0    60302 2020-02-02 00:00:00.000000 labneura-0.0.4/tests/assets/titanic.csv
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 labneura-0.0.4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 labneura-0.0.4/LICENSE
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 labneura-0.0.4/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 labneura-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 labneura-0.0.4/PKG-INFO
+drwxr-xr-x   0 gtk        (501) staff       (20)        0 2024-05-22 16:53:07.723651 labneura-0.0.5/
+-rw-r--r--   0 gtk        (501) staff       (20)        0 2024-05-22 16:03:39.000000 labneura-0.0.5/LICENCE
+-rw-r--r--   0 gtk        (501) staff       (20)      216 2024-05-22 16:53:07.723428 labneura-0.0.5/PKG-INFO
+-rw-r--r--   0 gtk        (501) staff       (20)        0 2024-05-22 16:03:34.000000 labneura-0.0.5/README.md
+drwxr-xr-x   0 gtk        (501) staff       (20)        0 2024-05-22 16:53:07.722339 labneura-0.0.5/labneura/
+-rw-r--r--   0 gtk        (501) staff       (20)        0 2024-05-22 16:04:17.000000 labneura-0.0.5/labneura/__init__.py
+drwxr-xr-x   0 gtk        (501) staff       (20)        0 2024-05-22 16:53:07.723226 labneura-0.0.5/labneura.egg-info/
+-rw-r--r--   0 gtk        (501) staff       (20)      216 2024-05-22 16:53:07.000000 labneura-0.0.5/labneura.egg-info/PKG-INFO
+-rw-r--r--   0 gtk        (501) staff       (20)      206 2024-05-22 16:53:07.000000 labneura-0.0.5/labneura.egg-info/SOURCES.txt
+-rw-r--r--   0 gtk        (501) staff       (20)        1 2024-05-22 16:53:07.000000 labneura-0.0.5/labneura.egg-info/dependency_links.txt
+-rw-r--r--   0 gtk        (501) staff       (20)        1 2024-05-22 16:10:41.000000 labneura-0.0.5/labneura.egg-info/not-zip-safe
+-rw-r--r--   0 gtk        (501) staff       (20)       19 2024-05-22 16:53:07.000000 labneura-0.0.5/labneura.egg-info/top_level.txt
+-rw-r--r--   0 gtk        (501) staff       (20)       38 2024-05-22 16:53:07.723691 labneura-0.0.5/setup.cfg
+-rw-r--r--   0 gtk        (501) staff       (20)     1639 2024-05-22 16:52:56.000000 labneura-0.0.5/setup.py
```

