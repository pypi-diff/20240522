# Comparing `tmp/pynenv-0.2.2.tar.gz` & `tmp/pynenv-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynenv-0.2.2.tar", max compression
+gzip compressed data, was "pynenv-0.2.3.tar", max compression
```

## Comparing `pynenv-0.2.2.tar` & `pynenv-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-05-21 06:38:02.002239 pynenv-0.2.2/LICENSE
--rw-r--r--   0        0        0      384 2024-05-22 17:40:28.797496 pynenv-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-05-21 06:49:05.377202 pynenv-0.2.2/pynenv/__init__.py
--rw-r--r--   0        0        0      911 2024-05-22 17:37:47.347698 pynenv-0.2.2/pynenv/environment.py
--rw-r--r--   0        0        0      323 2024-05-22 17:51:19.380687 pynenv-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 pynenv-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-21 06:38:02.002239 pynenv-0.2.3/LICENSE
+-rw-r--r--   0        0        0      384 2024-05-22 17:40:28.797496 pynenv-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 06:49:05.377202 pynenv-0.2.3/pynenv/__init__.py
+-rw-r--r--   0        0        0      911 2024-05-22 17:37:47.347698 pynenv-0.2.3/pynenv/environment.py
+-rw-r--r--   0        0        0      362 2024-05-22 17:56:20.487517 pynenv-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 pynenv-0.2.3/PKG-INFO
```

### Comparing `pynenv-0.2.2/LICENSE` & `pynenv-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynenv-0.2.2/pynenv/environment.py` & `pynenv-0.2.3/pynenv/environment.py`

 * *Files identical despite different names*

