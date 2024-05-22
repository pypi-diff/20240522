# Comparing `tmp/sentier_glossary-0.2.0.tar.gz` & `tmp/sentier_glossary-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentier_glossary-0.2.0.tar", last modified: Mon May 20 13:30:02 2024, max compression
+gzip compressed data, was "sentier_glossary-0.3.0.tar", last modified: Tue May 21 18:11:47 2024, max compression
```

## Comparing `sentier_glossary-0.2.0.tar` & `sentier_glossary-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:30:02.686800 sentier_glossary-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-20 13:29:59.000000 sentier_glossary-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:29:59.000000 sentier_glossary-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-20 13:30:02.686800 sentier_glossary-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-20 13:29:59.000000 sentier_glossary-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-20 13:29:59.000000 sentier_glossary-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:30:02.686800 sentier_glossary-0.2.0/sentier_glossary/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-20 13:29:59.000000 sentier_glossary-0.2.0/sentier_glossary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-05-20 13:29:59.000000 sentier_glossary-0.2.0/sentier_glossary/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-20 13:29:59.000000 sentier_glossary-0.2.0/sentier_glossary/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:30:02.686800 sentier_glossary-0.2.0/sentier_glossary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-20 13:30:02.000000 sentier_glossary-0.2.0/sentier_glossary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 13:30:02.000000 sentier_glossary-0.2.0/sentier_glossary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:30:02.000000 sentier_glossary-0.2.0/sentier_glossary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-20 13:30:02.000000 sentier_glossary-0.2.0/sentier_glossary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 13:30:02.000000 sentier_glossary-0.2.0/sentier_glossary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:30:02.686800 sentier_glossary-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:11:47.907541 sentier_glossary-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 18:11:44.000000 sentier_glossary-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:11:44.000000 sentier_glossary-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-21 18:11:47.907541 sentier_glossary-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-21 18:11:44.000000 sentier_glossary-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-21 18:11:44.000000 sentier_glossary-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:11:47.903541 sentier_glossary-0.3.0/sentier_glossary/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-21 18:11:44.000000 sentier_glossary-0.3.0/sentier_glossary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-05-21 18:11:44.000000 sentier_glossary-0.3.0/sentier_glossary/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-21 18:11:44.000000 sentier_glossary-0.3.0/sentier_glossary/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:11:47.903541 sentier_glossary-0.3.0/sentier_glossary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-21 18:11:47.000000 sentier_glossary-0.3.0/sentier_glossary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-21 18:11:47.000000 sentier_glossary-0.3.0/sentier_glossary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:11:47.000000 sentier_glossary-0.3.0/sentier_glossary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-21 18:11:47.000000 sentier_glossary-0.3.0/sentier_glossary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-21 18:11:47.000000 sentier_glossary-0.3.0/sentier_glossary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 18:11:47.907541 sentier_glossary-0.3.0/setup.cfg
```

### Comparing `sentier_glossary-0.2.0/LICENSE` & `sentier_glossary-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentier_glossary-0.2.0/pyproject.toml` & `sentier_glossary-0.3.0/pyproject.toml`

 * *Files identical despite different names*

