# Comparing `tmp/iceye_audit_log-0.1.0.tar.gz` & `tmp/iceye_audit_log-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceye_audit_log-0.1.0.tar", last modified: Mon May 20 08:38:46 2024, max compression
+gzip compressed data, was "iceye_audit_log-0.1.1.tar", last modified: Wed May 22 06:15:44 2024, max compression
```

## Comparing `iceye_audit_log-0.1.0.tar` & `iceye_audit_log-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:38:46.338806 iceye_audit_log-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:38:46.334806 iceye_audit_log-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:38:46.334806 iceye_audit_log-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-20 08:38:46.338806 iceye_audit_log-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:38:46.334806 iceye_audit_log-0.1.0/audit_log/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/audit_log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/audit_log/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/audit_log/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/audit_log/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/audit_log/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:38:46.338806 iceye_audit_log-0.1.0/iceye_audit_log.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-20 08:38:46.000000 iceye_audit_log-0.1.0/iceye_audit_log.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-20 08:38:46.000000 iceye_audit_log-0.1.0/iceye_audit_log.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:38:46.000000 iceye_audit_log-0.1.0/iceye_audit_log.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 08:38:46.000000 iceye_audit_log-0.1.0/iceye_audit_log.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:38:46.338806 iceye_audit_log-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:38:46.338806 iceye_audit_log-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-20 08:38:32.000000 iceye_audit_log-0.1.0/tests/test_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/audit_log/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/audit_log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/audit_log/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/audit_log/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/audit_log/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/audit_log/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/audit_log/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/iceye_audit_log.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-22 06:15:44.000000 iceye_audit_log-0.1.1/iceye_audit_log.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-22 06:15:44.000000 iceye_audit_log-0.1.1/iceye_audit_log.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 06:15:44.000000 iceye_audit_log-0.1.1/iceye_audit_log.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 06:15:44.000000 iceye_audit_log-0.1.1/iceye_audit_log.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/tests/test_log.py
```

### Comparing `iceye_audit_log-0.1.0/.github/workflows/release.yml` & `iceye_audit_log-0.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.0/.github/workflows/test.yml` & `iceye_audit_log-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.0/.gitignore` & `iceye_audit_log-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.0/.pre-commit-config.yaml` & `iceye_audit_log-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.0/LICENSE` & `iceye_audit_log-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.0/PKG-INFO` & `iceye_audit_log-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceye-audit-log
-Version: 0.1.0
+Version: 0.1.1
 Summary: Audit logging library for Python
 License: MIT License
         
         Copyright (c) 2024 Iceye Oy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `iceye_audit_log-0.1.0/SECURITY.md` & `iceye_audit_log-0.1.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.0/audit_log/headers.py` & `iceye_audit_log-0.1.1/audit_log/headers.py`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.0/audit_log/log.py` & `iceye_audit_log-0.1.1/audit_log/log.py`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.0/iceye_audit_log.egg-info/PKG-INFO` & `iceye_audit_log-0.1.1/iceye_audit_log.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceye-audit-log
-Version: 0.1.0
+Version: 0.1.1
 Summary: Audit logging library for Python
 License: MIT License
         
         Copyright (c) 2024 Iceye Oy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `iceye_audit_log-0.1.0/iceye_audit_log.egg-info/SOURCES.txt` & `iceye_audit_log-0.1.1/iceye_audit_log.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 .github/workflows/pre-commit.yml
 .github/workflows/release.yml
 .github/workflows/test.yml
 audit_log/__init__.py
 audit_log/exceptions.py
 audit_log/headers.py
 audit_log/log.py
+audit_log/py.typed
 audit_log/schema.py
 iceye_audit_log.egg-info/PKG-INFO
 iceye_audit_log.egg-info/SOURCES.txt
 iceye_audit_log.egg-info/dependency_links.txt
 iceye_audit_log.egg-info/top_level.txt
 tests/test_headers.py
 tests/test_log.py
```

### Comparing `iceye_audit_log-0.1.0/pyproject.toml` & `iceye_audit_log-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.0/tests/test_headers.py` & `iceye_audit_log-0.1.1/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.0/tests/test_log.py` & `iceye_audit_log-0.1.1/tests/test_log.py`

 * *Files identical despite different names*

