# Comparing `tmp/pih-doc-0.16.tar.gz` & `tmp/pih-doc-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-doc-0.16.tar", last modified: Mon May 20 23:02:04 2024, max compression
+gzip compressed data, was "pih-doc-0.17.tar", last modified: Tue May 21 19:20:19 2024, max compression
```

## Comparing `pih-doc-0.16.tar` & `pih-doc-0.17.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 23:02:05.010537 pih-doc-0.16/
-drwxrwxrwx   0        0        0        0 2024-05-20 23:02:04.541947 pih-doc-0.16/DocsService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-doc-0.16/DocsService/__init__.py
--rw-rw-rw-   0        0        0      146 2024-02-13 08:06:49.000000 pih-doc-0.16/DocsService/__main__.py
--rw-rw-rw-   0        0        0    41563 2024-05-06 00:47:28.000000 pih-doc-0.16/DocsService/api.py
--rw-rw-rw-   0        0        0     1634 2024-05-20 23:01:45.000000 pih-doc-0.16/DocsService/const.py
--rw-rw-rw-   0        0        0     5242 2024-05-20 23:01:06.000000 pih-doc-0.16/DocsService/service.py
--rw-rw-rw-   0        0        0      729 2024-02-17 13:43:10.000000 pih-doc-0.16/DocsService/tools.py
--rw-rw-rw-   0        0        0      595 2024-05-20 23:02:04.979287 pih-doc-0.16/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 23:02:04.948040 pih-doc-0.16/pih_doc.egg-info/
--rw-rw-rw-   0        0        0      595 2024-05-20 23:02:04.000000 pih-doc-0.16/pih_doc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-05-20 23:02:04.000000 pih-doc-0.16/pih_doc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 23:02:04.000000 pih-doc-0.16/pih_doc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-20 23:02:04.000000 pih-doc-0.16/pih_doc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      123 2024-05-20 23:02:04.000000 pih-doc-0.16/pih_doc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-20 23:02:04.000000 pih-doc-0.16/pih_doc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 23:02:05.026164 pih-doc-0.16/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 19:20:19.598162 pih-doc-0.17/
+drwxrwxrwx   0        0        0        0 2024-05-21 19:20:19.131886 pih-doc-0.17/DocsService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-doc-0.17/DocsService/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-02-13 08:06:49.000000 pih-doc-0.17/DocsService/__main__.py
+-rw-rw-rw-   0        0        0    41563 2024-05-06 00:47:28.000000 pih-doc-0.17/DocsService/api.py
+-rw-rw-rw-   0        0        0     1634 2024-05-21 19:20:04.000000 pih-doc-0.17/DocsService/const.py
+-rw-rw-rw-   0        0        0     5242 2024-05-20 23:01:06.000000 pih-doc-0.17/DocsService/service.py
+-rw-rw-rw-   0        0        0      729 2024-02-17 13:43:10.000000 pih-doc-0.17/DocsService/tools.py
+-rw-rw-rw-   0        0        0      595 2024-05-21 19:20:19.533547 pih-doc-0.17/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-21 19:20:19.486696 pih-doc-0.17/pih_doc.egg-info/
+-rw-rw-rw-   0        0        0      595 2024-05-21 19:20:18.000000 pih-doc-0.17/pih_doc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-05-21 19:20:18.000000 pih-doc-0.17/pih_doc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 19:20:18.000000 pih-doc-0.17/pih_doc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-21 19:20:18.000000 pih-doc-0.17/pih_doc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      123 2024-05-21 19:20:18.000000 pih-doc-0.17/pih_doc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 19:20:18.000000 pih-doc-0.17/pih_doc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 19:20:19.598162 pih-doc-0.17/setup.cfg
```

### Comparing `pih-doc-0.16/DocsService/api.py` & `pih-doc-0.17/DocsService/api.py`

 * *Files identical despite different names*

### Comparing `pih-doc-0.16/DocsService/const.py` & `pih-doc-0.17/DocsService/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     QUANTITY_COLUMN_NAME: str = "фактическое наличие"
     NAME_MAX_LENTH: int = 120
     QUANTITY_NOT_SET: str = "-"
 
 
 HOST = Hosts.DC2
 
-VERSION: str = "0.16"
+VERSION: str = "0.17"
 
 PACKAGES: tuple[str, ...] = (
     "xlsxwriter",
     "xlrd",
     "xlutils",
     "openpyxl",
     "python-barcode",
```

### Comparing `pih-doc-0.16/DocsService/service.py` & `pih-doc-0.17/DocsService/service.py`

 * *Files identical despite different names*

### Comparing `pih-doc-0.16/DocsService/tools.py` & `pih-doc-0.17/DocsService/tools.py`

 * *Files identical despite different names*

### Comparing `pih-doc-0.16/PKG-INFO` & `pih-doc-0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pih-doc
-Version: 0.16
+Version: 0.17
 Summary: PIH Documents service package
 Home-page: https://pacifichosp.com/
 Author: Nikita Karachentsev
 Author-email: it@pacifichosp.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: ipih
```

### Comparing `pih-doc-0.16/pih_doc.egg-info/PKG-INFO` & `pih-doc-0.17/pih_doc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pih-doc
-Version: 0.16
+Version: 0.17
 Summary: PIH Documents service package
 Home-page: https://pacifichosp.com/
 Author: Nikita Karachentsev
 Author-email: it@pacifichosp.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: ipih
```

