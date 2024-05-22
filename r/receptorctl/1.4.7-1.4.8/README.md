# Comparing `tmp/receptorctl-1.4.7.tar.gz` & `tmp/receptorctl-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "receptorctl-1.4.7.tar", last modified: Thu May  9 17:43:31 2024, max compression
+gzip compressed data, was "receptorctl-1.4.8.tar", last modified: Wed May 22 15:56:43 2024, max compression
```

## Comparing `receptorctl-1.4.7.tar` & `receptorctl-1.4.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:43:31.825975 receptorctl-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 17:43:22.000000 receptorctl-1.4.7/.VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-09 17:43:19.000000 receptorctl-1.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-09 17:43:31.825975 receptorctl-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-09 17:43:19.000000 receptorctl-1.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-09 17:43:19.000000 receptorctl-1.4.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:43:31.821975 receptorctl-1.4.7/receptorctl/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-09 17:43:19.000000 receptorctl-1.4.7/receptorctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 17:43:19.000000 receptorctl-1.4.7/receptorctl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-05-09 17:43:19.000000 receptorctl-1.4.7/receptorctl/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-05-09 17:43:19.000000 receptorctl-1.4.7/receptorctl/socket_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:43:31.825975 receptorctl-1.4.7/receptorctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-09 17:43:31.000000 receptorctl-1.4.7/receptorctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-09 17:43:31.000000 receptorctl-1.4.7/receptorctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:43:31.000000 receptorctl-1.4.7/receptorctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-09 17:43:31.000000 receptorctl-1.4.7/receptorctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-09 17:43:31.000000 receptorctl-1.4.7/receptorctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 17:43:31.000000 receptorctl-1.4.7/receptorctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-09 17:43:31.825975 receptorctl-1.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-09 17:43:19.000000 receptorctl-1.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:43:31.825975 receptorctl-1.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-09 17:43:19.000000 receptorctl-1.4.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-05-09 17:43:19.000000 receptorctl-1.4.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-09 17:43:19.000000 receptorctl-1.4.7/tests/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-09 17:43:19.000000 receptorctl-1.4.7/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-09 17:43:19.000000 receptorctl-1.4.7/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-09 17:43:19.000000 receptorctl-1.4.7/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-09 17:43:19.000000 receptorctl-1.4.7/tests/test_workunit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:56:43.124773 receptorctl-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 15:56:33.000000 receptorctl-1.4.8/.VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-22 15:56:29.000000 receptorctl-1.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-22 15:56:43.124773 receptorctl-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-22 15:56:29.000000 receptorctl-1.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-22 15:56:29.000000 receptorctl-1.4.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:56:43.124773 receptorctl-1.4.8/receptorctl/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-22 15:56:29.000000 receptorctl-1.4.8/receptorctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 15:56:29.000000 receptorctl-1.4.8/receptorctl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-05-22 15:56:29.000000 receptorctl-1.4.8/receptorctl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-05-22 15:56:29.000000 receptorctl-1.4.8/receptorctl/socket_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:56:43.124773 receptorctl-1.4.8/receptorctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-22 15:56:43.000000 receptorctl-1.4.8/receptorctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-22 15:56:43.000000 receptorctl-1.4.8/receptorctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:56:43.000000 receptorctl-1.4.8/receptorctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-22 15:56:43.000000 receptorctl-1.4.8/receptorctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 15:56:43.000000 receptorctl-1.4.8/receptorctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 15:56:43.000000 receptorctl-1.4.8/receptorctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-22 15:56:43.124773 receptorctl-1.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-22 15:56:29.000000 receptorctl-1.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:56:43.124773 receptorctl-1.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-22 15:56:29.000000 receptorctl-1.4.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-05-22 15:56:29.000000 receptorctl-1.4.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-22 15:56:29.000000 receptorctl-1.4.8/tests/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-22 15:56:29.000000 receptorctl-1.4.8/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-22 15:56:29.000000 receptorctl-1.4.8/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-22 15:56:29.000000 receptorctl-1.4.8/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-22 15:56:29.000000 receptorctl-1.4.8/tests/test_workunit.py
```

### Comparing `receptorctl-1.4.7/README.md` & `receptorctl-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.7/receptorctl/cli.py` & `receptorctl-1.4.8/receptorctl/cli.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.7/receptorctl/socket_interface.py` & `receptorctl-1.4.8/receptorctl/socket_interface.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.7/setup.cfg` & `receptorctl-1.4.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.7/tests/conftest.py` & `receptorctl-1.4.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.7/tests/lib.py` & `receptorctl-1.4.8/tests/lib.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.7/tests/test_cli.py` & `receptorctl-1.4.8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.7/tests/test_connection.py` & `receptorctl-1.4.8/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.7/tests/test_mesh.py` & `receptorctl-1.4.8/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.7/tests/test_workunit.py` & `receptorctl-1.4.8/tests/test_workunit.py`

 * *Files identical despite different names*

