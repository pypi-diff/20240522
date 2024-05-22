# Comparing `tmp/teklia-toolbox-0.1.4rc4.tar.gz` & `tmp/teklia_toolbox-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teklia-toolbox-0.1.4rc4.tar", last modified: Thu Mar 28 15:53:59 2024, max compression
+gzip compressed data, was "teklia_toolbox-0.1.5.tar", last modified: Wed May 22 14:51:57 2024, max compression
```

## Comparing `teklia-toolbox-0.1.4rc4.tar` & `teklia_toolbox-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:53:59.825969 teklia-toolbox-0.1.4rc4/
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-28 14:11:38.000000 teklia-toolbox-0.1.4rc4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      259 2024-03-28 15:53:59.821969 teklia-toolbox-0.1.4rc4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4142 2024-03-28 14:11:38.000000 teklia-toolbox-0.1.4rc4/README.md
--rw-rw-rw-   0 root         (0) root         (0)        9 2024-03-28 15:53:04.000000 teklia-toolbox-0.1.4rc4/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      713 2024-03-28 14:11:38.000000 teklia-toolbox-0.1.4rc4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       66 2024-03-28 14:26:40.000000 teklia-toolbox-0.1.4rc4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-28 15:53:59.825969 teklia-toolbox-0.1.4rc4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-03-28 14:11:38.000000 teklia-toolbox-0.1.4rc4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:53:59.821969 teklia-toolbox-0.1.4rc4/teklia_toolbox/
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-03-28 14:11:38.000000 teklia-toolbox-0.1.4rc4/teklia_toolbox/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4082 2024-03-28 14:11:38.000000 teklia-toolbox-0.1.4rc4/teklia_toolbox/config.py
--rw-rw-rw-   0 root         (0) root         (0)     6972 2024-03-28 14:11:38.000000 teklia-toolbox-0.1.4rc4/teklia_toolbox/pagexml.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2024-03-28 14:11:38.000000 teklia-toolbox-0.1.4rc4/teklia_toolbox/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-03-28 14:11:38.000000 teklia-toolbox-0.1.4rc4/teklia_toolbox/time.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2024-03-28 14:11:38.000000 teklia-toolbox-0.1.4rc4/teklia_toolbox/xml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:53:59.821969 teklia-toolbox-0.1.4rc4/teklia_toolbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)      259 2024-03-28 15:53:59.000000 teklia-toolbox-0.1.4rc4/teklia_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      494 2024-03-28 15:53:59.000000 teklia-toolbox-0.1.4rc4/teklia_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 15:53:59.000000 teklia-toolbox-0.1.4rc4/teklia_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-28 15:53:59.000000 teklia-toolbox-0.1.4rc4/teklia_toolbox.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-28 15:53:59.000000 teklia-toolbox-0.1.4rc4/teklia_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:53:59.821969 teklia-toolbox-0.1.4rc4/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3232 2024-03-28 14:11:38.000000 teklia-toolbox-0.1.4rc4/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     8750 2024-03-28 14:26:40.000000 teklia-toolbox-0.1.4rc4/tests/test_pagexml.py
--rw-rw-rw-   0 root         (0) root         (0)     1698 2024-03-28 14:11:38.000000 teklia-toolbox-0.1.4rc4/tests/test_requests.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-03-28 14:11:38.000000 teklia-toolbox-0.1.4rc4/tests/test_time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:51:57.657339 teklia_toolbox-0.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-22 14:51:03.000000 teklia_toolbox-0.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      225 2024-05-22 14:51:57.657339 teklia_toolbox-0.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4142 2024-05-22 14:51:03.000000 teklia_toolbox-0.1.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-22 14:51:03.000000 teklia_toolbox-0.1.5/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      713 2024-05-22 14:51:03.000000 teklia_toolbox-0.1.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-22 14:51:03.000000 teklia_toolbox-0.1.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 14:51:57.657339 teklia_toolbox-0.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-22 14:51:03.000000 teklia_toolbox-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:51:57.657339 teklia_toolbox-0.1.5/teklia_toolbox/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-05-22 14:51:03.000000 teklia_toolbox-0.1.5/teklia_toolbox/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4082 2024-05-22 14:51:03.000000 teklia_toolbox-0.1.5/teklia_toolbox/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6972 2024-05-22 14:51:03.000000 teklia_toolbox-0.1.5/teklia_toolbox/pagexml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2024-05-22 14:51:03.000000 teklia_toolbox-0.1.5/teklia_toolbox/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-22 14:51:03.000000 teklia_toolbox-0.1.5/teklia_toolbox/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2024-05-22 14:51:03.000000 teklia_toolbox-0.1.5/teklia_toolbox/xml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:51:57.657339 teklia_toolbox-0.1.5/teklia_toolbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      225 2024-05-22 14:51:57.000000 teklia_toolbox-0.1.5/teklia_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-22 14:51:57.000000 teklia_toolbox-0.1.5/teklia_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 14:51:57.000000 teklia_toolbox-0.1.5/teklia_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-22 14:51:57.000000 teklia_toolbox-0.1.5/teklia_toolbox.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-22 14:51:57.000000 teklia_toolbox-0.1.5/teklia_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:51:57.657339 teklia_toolbox-0.1.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3232 2024-05-22 14:51:03.000000 teklia_toolbox-0.1.5/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8750 2024-05-22 14:51:03.000000 teklia_toolbox-0.1.5/tests/test_pagexml.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2024-05-22 14:51:03.000000 teklia_toolbox-0.1.5/tests/test_time.py
```

### Comparing `teklia-toolbox-0.1.4rc4/README.md` & `teklia_toolbox-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `teklia-toolbox-0.1.4rc4/pyproject.toml` & `teklia_toolbox-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `teklia-toolbox-0.1.4rc4/setup.py` & `teklia_toolbox-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `teklia-toolbox-0.1.4rc4/teklia_toolbox/config.py` & `teklia_toolbox-0.1.5/teklia_toolbox/config.py`

 * *Files identical despite different names*

### Comparing `teklia-toolbox-0.1.4rc4/teklia_toolbox/pagexml.py` & `teklia_toolbox-0.1.5/teklia_toolbox/pagexml.py`

 * *Files identical despite different names*

### Comparing `teklia-toolbox-0.1.4rc4/teklia_toolbox/xml.py` & `teklia_toolbox-0.1.5/teklia_toolbox/xml.py`

 * *Files identical despite different names*

### Comparing `teklia-toolbox-0.1.4rc4/tests/test_config.py` & `teklia_toolbox-0.1.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `teklia-toolbox-0.1.4rc4/tests/test_pagexml.py` & `teklia_toolbox-0.1.5/tests/test_pagexml.py`

 * *Files identical despite different names*

