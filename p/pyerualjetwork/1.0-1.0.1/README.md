# Comparing `tmp/pyerualjetwork-1.0.tar.gz` & `tmp/pyerualjetwork-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.0.tar", last modified: Wed May 22 18:34:49 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.0.1.tar", last modified: Wed May 22 18:48:21 2024, max compression
```

## Comparing `pyerualjetwork-1.0.tar` & `pyerualjetwork-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 18:34:49.627372 pyerualjetwork-1.0/
--rw-rw-rw-   0        0        0      274 2024-05-22 18:34:49.627372 pyerualjetwork-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 18:34:49.623368 pyerualjetwork-1.0/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      274 2024-05-22 18:34:49.000000 pyerualjetwork-1.0/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2024-05-22 18:34:49.000000 pyerualjetwork-1.0/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 18:34:49.000000 pyerualjetwork-1.0/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 18:34:49.000000 pyerualjetwork-1.0/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 18:34:49.627372 pyerualjetwork-1.0/setup.cfg
--rw-rw-rw-   0        0        0      450 2024-05-22 18:01:51.000000 pyerualjetwork-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:48:21.868971 pyerualjetwork-1.0.1/
+-rw-rw-rw-   0        0        0      276 2024-05-22 18:48:21.866976 pyerualjetwork-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 18:48:21.864981 pyerualjetwork-1.0.1/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      276 2024-05-22 18:48:21.000000 pyerualjetwork-1.0.1/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2024-05-22 18:48:21.000000 pyerualjetwork-1.0.1/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 18:48:21.000000 pyerualjetwork-1.0.1/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 18:48:21.000000 pyerualjetwork-1.0.1/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 18:48:21.868971 pyerualjetwork-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-22 18:45:55.000000 pyerualjetwork-1.0.1/setup.py
```

