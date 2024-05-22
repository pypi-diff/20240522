# Comparing `tmp/meetsam-0.0.1.tar.gz` & `tmp/meetsam-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meetsam-0.0.1.tar", last modified: Thu May  2 02:52:15 2024, max compression
+gzip compressed data, was "meetsam-0.0.2.tar", last modified: Wed May 22 01:40:28 2024, max compression
```

## Comparing `meetsam-0.0.1.tar` & `meetsam-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:52:15.641770 meetsam-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-02 02:52:11.000000 meetsam-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-02 02:52:15.641770 meetsam-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-02 02:52:11.000000 meetsam-0.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-02 02:52:11.000000 meetsam-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 02:52:15.641770 meetsam-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:52:15.641770 meetsam-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:52:15.641770 meetsam-0.0.1/src/meetSam/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 02:52:11.000000 meetsam-0.0.1/src/meetSam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 02:52:11.000000 meetsam-0.0.1/src/meetSam/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-02 02:52:11.000000 meetsam-0.0.1/src/meetSam/meet_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:52:15.641770 meetsam-0.0.1/src/meetSam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-02 02:52:15.000000 meetsam-0.0.1/src/meetSam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-02 02:52:15.000000 meetsam-0.0.1/src/meetSam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 02:52:15.000000 meetsam-0.0.1/src/meetSam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 02:52:15.000000 meetsam-0.0.1/src/meetSam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:40:28.378165 meetsam-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-22 01:40:21.000000 meetsam-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-22 01:40:28.378165 meetsam-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-22 01:40:21.000000 meetsam-0.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-22 01:40:21.000000 meetsam-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:40:28.378165 meetsam-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:40:28.374165 meetsam-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:40:28.378165 meetsam-0.0.2/src/meetSam/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 01:40:21.000000 meetsam-0.0.2/src/meetSam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 01:40:21.000000 meetsam-0.0.2/src/meetSam/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-22 01:40:21.000000 meetsam-0.0.2/src/meetSam/meet_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:40:28.378165 meetsam-0.0.2/src/meetSam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-22 01:40:28.000000 meetsam-0.0.2/src/meetSam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-22 01:40:28.000000 meetsam-0.0.2/src/meetSam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:40:28.000000 meetsam-0.0.2/src/meetSam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 01:40:28.000000 meetsam-0.0.2/src/meetSam.egg-info/top_level.txt
```

### Comparing `meetsam-0.0.1/LICENSE` & `meetsam-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meetsam-0.0.1/src/meetSam/meet_sam.py` & `meetsam-0.0.2/src/meetSam/meet_sam.py`

 * *Files identical despite different names*

