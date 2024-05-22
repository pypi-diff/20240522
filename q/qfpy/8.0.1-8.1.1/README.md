# Comparing `tmp/qfpy-8.0.1.tar.gz` & `tmp/qfpy-8.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfpy-8.0.1.tar", last modified: Thu May  2 05:55:45 2024, max compression
+gzip compressed data, was "qfpy-8.1.1.tar", last modified: Wed May 22 17:34:34 2024, max compression
```

## Comparing `qfpy-8.0.1.tar` & `qfpy-8.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 05:55:45.484305 qfpy-8.0.1/
--rw-rw-rw-   0        0        0      229 2024-05-02 05:55:45.481434 qfpy-8.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-02 05:55:33.000000 qfpy-8.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-02 05:55:45.484305 qfpy-8.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-02 05:55:45.447538 qfpy-8.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-02 05:55:45.469097 qfpy-8.0.1/src/qfpy/
--rw-rw-rw-   0        0        0       90 2024-04-30 18:19:38.000000 qfpy-8.0.1/src/qfpy/__init__.py
--rw-rw-rw-   0        0        0      210 2024-04-29 16:48:36.000000 qfpy-8.0.1/src/qfpy/character.py
--rw-rw-rw-   0        0        0      131 2024-04-29 17:01:55.000000 qfpy-8.0.1/src/qfpy/crypto.py
--rw-rw-rw-   0        0        0     1528 2024-04-29 16:50:05.000000 qfpy-8.0.1/src/qfpy/exif.py
--rw-rw-rw-   0        0        0     2988 2024-05-02 05:54:03.000000 qfpy-8.0.1/src/qfpy/ffmpeg.py
--rw-rw-rw-   0        0        0      700 2024-04-29 16:53:48.000000 qfpy-8.0.1/src/qfpy/folder.py
--rw-rw-rw-   0        0        0      881 2024-04-29 16:55:19.000000 qfpy-8.0.1/src/qfpy/function.py
--rw-rw-rw-   0        0        0     1170 2024-04-30 18:20:15.000000 qfpy-8.0.1/src/qfpy/process.py
--rw-rw-rw-   0        0        0      525 2024-04-30 18:24:38.000000 qfpy-8.0.1/src/qfpy/system.py
-drwxrwxrwx   0        0        0        0 2024-05-02 05:55:45.479839 qfpy-8.0.1/src/qfpy.egg-info/
--rw-rw-rw-   0        0        0      229 2024-05-02 05:55:45.000000 qfpy-8.0.1/src/qfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2024-05-02 05:55:45.000000 qfpy-8.0.1/src/qfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 05:55:45.000000 qfpy-8.0.1/src/qfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-02 05:55:45.000000 qfpy-8.0.1/src/qfpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-02 05:55:45.000000 qfpy-8.0.1/src/qfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 17:34:34.154251 qfpy-8.1.1/
+-rw-rw-rw-   0        0        0      229 2024-05-22 17:34:34.152292 qfpy-8.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-22 17:34:11.000000 qfpy-8.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 17:34:34.154251 qfpy-8.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 17:34:34.125931 qfpy-8.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 17:34:34.141556 qfpy-8.1.1/src/qfpy/
+-rw-rw-rw-   0        0        0       90 2024-04-30 18:19:38.000000 qfpy-8.1.1/src/qfpy/__init__.py
+-rw-rw-rw-   0        0        0      210 2024-04-29 16:48:36.000000 qfpy-8.1.1/src/qfpy/character.py
+-rw-rw-rw-   0        0        0      562 2024-05-22 17:34:06.000000 qfpy-8.1.1/src/qfpy/crypto.py
+-rw-rw-rw-   0        0        0     1528 2024-04-29 16:50:05.000000 qfpy-8.1.1/src/qfpy/exif.py
+-rw-rw-rw-   0        0        0     2988 2024-05-02 05:54:03.000000 qfpy-8.1.1/src/qfpy/ffmpeg.py
+-rw-rw-rw-   0        0        0      700 2024-04-29 16:53:48.000000 qfpy-8.1.1/src/qfpy/folder.py
+-rw-rw-rw-   0        0        0      881 2024-04-29 16:55:19.000000 qfpy-8.1.1/src/qfpy/function.py
+-rw-rw-rw-   0        0        0     1170 2024-04-30 18:20:15.000000 qfpy-8.1.1/src/qfpy/process.py
+-rw-rw-rw-   0        0        0      525 2024-04-30 18:24:38.000000 qfpy-8.1.1/src/qfpy/system.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:34:34.151320 qfpy-8.1.1/src/qfpy.egg-info/
+-rw-rw-rw-   0        0        0      229 2024-05-22 17:34:34.000000 qfpy-8.1.1/src/qfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2024-05-22 17:34:34.000000 qfpy-8.1.1/src/qfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 17:34:34.000000 qfpy-8.1.1/src/qfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-22 17:34:34.000000 qfpy-8.1.1/src/qfpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 17:34:34.000000 qfpy-8.1.1/src/qfpy.egg-info/top_level.txt
```

### Comparing `qfpy-8.0.1/src/qfpy/exif.py` & `qfpy-8.1.1/src/qfpy/exif.py`

 * *Files identical despite different names*

### Comparing `qfpy-8.0.1/src/qfpy/ffmpeg.py` & `qfpy-8.1.1/src/qfpy/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `qfpy-8.0.1/src/qfpy/folder.py` & `qfpy-8.1.1/src/qfpy/folder.py`

 * *Files identical despite different names*

### Comparing `qfpy-8.0.1/src/qfpy/function.py` & `qfpy-8.1.1/src/qfpy/function.py`

 * *Files identical despite different names*

### Comparing `qfpy-8.0.1/src/qfpy/process.py` & `qfpy-8.1.1/src/qfpy/process.py`

 * *Files identical despite different names*

### Comparing `qfpy-8.0.1/src/qfpy/system.py` & `qfpy-8.1.1/src/qfpy/system.py`

 * *Files identical despite different names*

