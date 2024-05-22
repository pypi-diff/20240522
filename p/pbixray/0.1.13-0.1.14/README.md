# Comparing `tmp/pbixray-0.1.13.tar.gz` & `tmp/pbixray-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbixray-0.1.13.tar", last modified: Fri May 17 23:28:52 2024, max compression
+gzip compressed data, was "pbixray-0.1.14.tar", last modified: Wed May 22 09:52:29 2024, max compression
```

## Comparing `pbixray-0.1.13.tar` & `pbixray-0.1.14.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 23:28:52.854069 pbixray-0.1.13/
--rw-rw-rw-   0        0        0     1069 2024-05-13 17:31:25.000000 pbixray-0.1.13/LICENSE
--rw-rw-rw-   0        0        0      109 2023-10-30 14:32:24.000000 pbixray-0.1.13/MANIFEST.in
--rw-rw-rw-   0        0        0     3639 2024-05-17 23:28:52.852071 pbixray-0.1.13/PKG-INFO
--rw-rw-rw-   0        0        0     2440 2024-05-15 22:12:16.000000 pbixray-0.1.13/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 23:28:52.717754 pbixray-0.1.13/pbixray/
--rw-rw-rw-   0        0        0       27 2023-10-23 09:05:31.000000 pbixray-0.1.13/pbixray/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 23:28:52.777078 pbixray-0.1.13/pbixray/abf/
--rw-rw-rw-   0        0        0        0 2023-10-06 13:44:17.000000 pbixray-0.1.13/pbixray/abf/__init__.py
--rw-rw-rw-   0        0        0     2528 2023-10-20 15:40:22.000000 pbixray-0.1.13/pbixray/abf/backup_log.py
--rw-rw-rw-   0        0        0     1311 2023-10-06 16:35:04.000000 pbixray-0.1.13/pbixray/abf/backup_log_header.py
--rw-rw-rw-   0        0        0      147 2023-10-24 17:14:37.000000 pbixray-0.1.13/pbixray/abf/data_model.py
--rw-rw-rw-   0        0        0     2940 2023-10-24 17:41:21.000000 pbixray-0.1.13/pbixray/abf/parser.py
--rw-rw-rw-   0        0        0      835 2023-10-04 17:01:32.000000 pbixray-0.1.13/pbixray/abf/virtual_directory.py
-drwxrwxrwx   0        0        0        0 2024-05-17 23:28:52.787804 pbixray-0.1.13/pbixray/column_data/
--rw-rw-rw-   0        0        0        0 2023-10-06 13:44:27.000000 pbixray-0.1.13/pbixray/column_data/__init__.py
--rw-rw-rw-   0        0        0    10091 2024-05-16 15:46:03.000000 pbixray-0.1.13/pbixray/column_data/dictionary.py
--rw-rw-rw-   0        0        0     3914 2023-09-26 13:03:34.000000 pbixray-0.1.13/pbixray/column_data/hidx.py
--rw-rw-rw-   0        0        0     1928 2023-09-20 13:58:20.000000 pbixray-0.1.13/pbixray/column_data/idf.py
--rw-rw-rw-   0        0        0     9004 2023-10-07 22:06:30.000000 pbixray-0.1.13/pbixray/column_data/idfmeta.py
--rw-rw-rw-   0        0        0     1514 2023-10-24 17:34:41.000000 pbixray-0.1.13/pbixray/core.py
--rw-rw-rw-   0        0        0     2605 2024-05-16 15:44:29.000000 pbixray-0.1.13/pbixray/huffman.py
-drwxrwxrwx   0        0        0        0 2024-05-17 23:28:52.812638 pbixray-0.1.13/pbixray/lib/
--rw-rw-rw-   0        0        0    49664 2023-10-16 14:51:50.000000 pbixray-0.1.13/pbixray/lib/libxpress9.dll
--rw-rw-rw-   0        0        0    68653 2023-10-30 15:56:31.000000 pbixray-0.1.13/pbixray/lib/libxpress9.dylib
--rw-rw-rw-   0        0        0    72376 2023-10-16 14:50:50.000000 pbixray-0.1.13/pbixray/lib/libxpress9.so
-drwxrwxrwx   0        0        0        0 2024-05-17 23:28:52.835178 pbixray-0.1.13/pbixray/meta/
--rw-rw-rw-   0        0        0        0 2023-10-06 15:24:30.000000 pbixray-0.1.13/pbixray/meta/__init__.py
--rw-rw-rw-   0        0        0     2186 2023-10-24 17:46:02.000000 pbixray-0.1.13/pbixray/meta/metadata_handler.py
--rw-rw-rw-   0        0        0     2869 2024-05-17 16:46:58.000000 pbixray-0.1.13/pbixray/meta/metadata_query.py
--rw-rw-rw-   0        0        0     1188 2023-10-23 16:34:31.000000 pbixray-0.1.13/pbixray/meta/sqlite_handler.py
--rw-rw-rw-   0        0        0     4042 2023-10-30 14:34:30.000000 pbixray-0.1.13/pbixray/pbix_unpacker.py
--rw-rw-rw-   0        0        0      955 2023-10-24 17:20:54.000000 pbixray-0.1.13/pbixray/utils.py
--rw-rw-rw-   0        0        0     9739 2024-05-17 23:28:17.000000 pbixray-0.1.13/pbixray/vertipaq_decoder.py
-drwxrwxrwx   0        0        0        0 2024-05-17 23:28:52.851033 pbixray-0.1.13/pbixray.egg-info/
--rw-rw-rw-   0        0        0     3639 2024-05-17 23:28:52.000000 pbixray-0.1.13/pbixray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      864 2024-05-17 23:28:52.000000 pbixray-0.1.13/pbixray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 23:28:52.000000 pbixray-0.1.13/pbixray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-17 23:28:52.000000 pbixray-0.1.13/pbixray.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-17 23:28:52.000000 pbixray-0.1.13/pbixray.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 23:28:52.854069 pbixray-0.1.13/setup.cfg
--rw-rw-rw-   0        0        0     1492 2024-05-17 23:27:41.000000 pbixray-0.1.13/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 23:28:52.845749 pbixray-0.1.13/test/
--rw-rw-rw-   0        0        0      975 2024-05-17 11:06:45.000000 pbixray-0.1.13/test/test_basic_operation.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:52:29.567077 pbixray-0.1.14/
+-rw-rw-rw-   0        0        0     1069 2024-05-13 17:31:25.000000 pbixray-0.1.14/LICENSE
+-rw-rw-rw-   0        0        0      109 2023-10-30 14:32:24.000000 pbixray-0.1.14/MANIFEST.in
+-rw-rw-rw-   0        0        0     3710 2024-05-22 09:52:29.567077 pbixray-0.1.14/PKG-INFO
+-rw-rw-rw-   0        0        0     2511 2024-05-20 13:43:08.000000 pbixray-0.1.14/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 09:52:29.472852 pbixray-0.1.14/pbixray/
+-rw-rw-rw-   0        0        0       27 2023-10-23 09:05:31.000000 pbixray-0.1.14/pbixray/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:52:29.526397 pbixray-0.1.14/pbixray/abf/
+-rw-rw-rw-   0        0        0        0 2023-10-06 13:44:17.000000 pbixray-0.1.14/pbixray/abf/__init__.py
+-rw-rw-rw-   0        0        0     2528 2023-10-20 15:40:22.000000 pbixray-0.1.14/pbixray/abf/backup_log.py
+-rw-rw-rw-   0        0        0     1311 2023-10-06 16:35:04.000000 pbixray-0.1.14/pbixray/abf/backup_log_header.py
+-rw-rw-rw-   0        0        0      147 2023-10-24 17:14:37.000000 pbixray-0.1.14/pbixray/abf/data_model.py
+-rw-rw-rw-   0        0        0     2940 2023-10-24 17:41:21.000000 pbixray-0.1.14/pbixray/abf/parser.py
+-rw-rw-rw-   0        0        0      835 2023-10-04 17:01:32.000000 pbixray-0.1.14/pbixray/abf/virtual_directory.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:52:29.530949 pbixray-0.1.14/pbixray/column_data/
+-rw-rw-rw-   0        0        0        0 2023-10-06 13:44:27.000000 pbixray-0.1.14/pbixray/column_data/__init__.py
+-rw-rw-rw-   0        0        0    10091 2024-05-16 15:46:03.000000 pbixray-0.1.14/pbixray/column_data/dictionary.py
+-rw-rw-rw-   0        0        0     3914 2023-09-26 13:03:34.000000 pbixray-0.1.14/pbixray/column_data/hidx.py
+-rw-rw-rw-   0        0        0     1928 2023-09-20 13:58:20.000000 pbixray-0.1.14/pbixray/column_data/idf.py
+-rw-rw-rw-   0        0        0     9004 2023-10-07 22:06:30.000000 pbixray-0.1.14/pbixray/column_data/idfmeta.py
+-rw-rw-rw-   0        0        0     1514 2023-10-24 17:34:41.000000 pbixray-0.1.14/pbixray/core.py
+-rw-rw-rw-   0        0        0     2605 2024-05-16 15:44:29.000000 pbixray-0.1.14/pbixray/huffman.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:52:29.551255 pbixray-0.1.14/pbixray/lib/
+-rw-rw-rw-   0        0        0    49664 2023-10-16 14:51:50.000000 pbixray-0.1.14/pbixray/lib/libxpress9.dll
+-rw-rw-rw-   0        0        0    68653 2023-10-30 15:56:31.000000 pbixray-0.1.14/pbixray/lib/libxpress9.dylib
+-rw-rw-rw-   0        0        0    72376 2023-10-16 14:50:50.000000 pbixray-0.1.14/pbixray/lib/libxpress9.so
+drwxrwxrwx   0        0        0        0 2024-05-22 09:52:29.555699 pbixray-0.1.14/pbixray/meta/
+-rw-rw-rw-   0        0        0        0 2023-10-06 15:24:30.000000 pbixray-0.1.14/pbixray/meta/__init__.py
+-rw-rw-rw-   0        0        0     2186 2023-10-24 17:46:02.000000 pbixray-0.1.14/pbixray/meta/metadata_handler.py
+-rw-rw-rw-   0        0        0     2869 2024-05-17 16:46:58.000000 pbixray-0.1.14/pbixray/meta/metadata_query.py
+-rw-rw-rw-   0        0        0     1188 2023-10-23 16:34:31.000000 pbixray-0.1.14/pbixray/meta/sqlite_handler.py
+-rw-rw-rw-   0        0        0     4042 2023-10-30 14:34:30.000000 pbixray-0.1.14/pbixray/pbix_unpacker.py
+-rw-rw-rw-   0        0        0      955 2024-05-22 09:49:40.000000 pbixray-0.1.14/pbixray/utils.py
+-rw-rw-rw-   0        0        0     9739 2024-05-17 23:28:17.000000 pbixray-0.1.14/pbixray/vertipaq_decoder.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:52:29.567077 pbixray-0.1.14/pbixray.egg-info/
+-rw-rw-rw-   0        0        0     3710 2024-05-22 09:52:29.000000 pbixray-0.1.14/pbixray.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2024-05-22 09:52:29.000000 pbixray-0.1.14/pbixray.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 09:52:29.000000 pbixray-0.1.14/pbixray.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-22 09:52:29.000000 pbixray-0.1.14/pbixray.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-22 09:52:29.000000 pbixray-0.1.14/pbixray.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 09:52:29.567077 pbixray-0.1.14/setup.cfg
+-rw-rw-rw-   0        0        0     1492 2024-05-22 09:51:51.000000 pbixray-0.1.14/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:52:29.566024 pbixray-0.1.14/test/
+-rw-rw-rw-   0        0        0      975 2024-05-17 11:06:45.000000 pbixray-0.1.14/test/test_basic_operation.py
```

### Comparing `pbixray-0.1.13/LICENSE` & `pbixray-0.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/PKG-INFO` & `pbixray-0.1.14/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbixray
-Version: 0.1.13
+Version: 0.1.14
 Summary: A Python library to parse and analyze PBIX files used with Microsoft Power BI.
 Home-page: https://github.com/Hugoberry/pbixray
 Author: Igor Cotruta
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -24,25 +24,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: kaitaistruct
 Requires-Dist: pandas
 Requires-Dist: apsw
 
 # PBIXRay
-
+[![Downloads](https://static.pepy.tech/badge/pbixray)](https://pepy.tech/project/pbixray)
 ## Overview
 
 PBIXRay is a Python library designed to parse and analyze PBIX files, which are used with Microsoft Power BI. This library provides a straightforward way to extract valuable information from PBIX files, including tables, metadata, Power Query code, and more.
 
 ## Installation
 
 Before using PBIXRay, ensure you have the following Python modules installed: `apsw`, `kaitaistruct`, and `pbixray`. You can install them using pip:
 
 ```bash
-pip install apsw kaitaistruct pbixray
+pip install pbixray
 ```
 
 ## Getting Started
 To start using PBIXRay, import the module and initialize it with the path to your PBIX file:
 ```python
 from pbixray import PBIXRay
```

### Comparing `pbixray-0.1.13/README.md` & `pbixray-0.1.14/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # PBIXRay
-
+[![Downloads](https://static.pepy.tech/badge/pbixray)](https://pepy.tech/project/pbixray)
 ## Overview
 
 PBIXRay is a Python library designed to parse and analyze PBIX files, which are used with Microsoft Power BI. This library provides a straightforward way to extract valuable information from PBIX files, including tables, metadata, Power Query code, and more.
 
 ## Installation
 
 Before using PBIXRay, ensure you have the following Python modules installed: `apsw`, `kaitaistruct`, and `pbixray`. You can install them using pip:
 
 ```bash
-pip install apsw kaitaistruct pbixray
+pip install pbixray
 ```
 
 ## Getting Started
 To start using PBIXRay, import the module and initialize it with the path to your PBIX file:
 ```python
 from pbixray import PBIXRay
```

### Comparing `pbixray-0.1.13/pbixray/abf/backup_log.py` & `pbixray-0.1.14/pbixray/abf/backup_log.py`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/abf/backup_log_header.py` & `pbixray-0.1.14/pbixray/abf/backup_log_header.py`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/abf/parser.py` & `pbixray-0.1.14/pbixray/abf/parser.py`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/abf/virtual_directory.py` & `pbixray-0.1.14/pbixray/abf/virtual_directory.py`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/column_data/dictionary.py` & `pbixray-0.1.14/pbixray/column_data/dictionary.py`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/column_data/hidx.py` & `pbixray-0.1.14/pbixray/column_data/hidx.py`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/column_data/idf.py` & `pbixray-0.1.14/pbixray/column_data/idf.py`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/column_data/idfmeta.py` & `pbixray-0.1.14/pbixray/column_data/idfmeta.py`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/core.py` & `pbixray-0.1.14/pbixray/core.py`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/huffman.py` & `pbixray-0.1.14/pbixray/huffman.py`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/lib/libxpress9.dll` & `pbixray-0.1.14/pbixray/lib/libxpress9.dll`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/lib/libxpress9.dylib` & `pbixray-0.1.14/pbixray/lib/libxpress9.dylib`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/lib/libxpress9.so` & `pbixray-0.1.14/pbixray/lib/libxpress9.so`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/meta/metadata_handler.py` & `pbixray-0.1.14/pbixray/meta/metadata_handler.py`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/meta/metadata_query.py` & `pbixray-0.1.14/pbixray/meta/metadata_query.py`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/meta/sqlite_handler.py` & `pbixray-0.1.14/pbixray/meta/sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/pbix_unpacker.py` & `pbixray-0.1.14/pbixray/pbix_unpacker.py`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray/utils.py` & `pbixray-0.1.14/pbixray/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .abf.data_model import DataModel
 
 # ---------- CONSTANTS ----------
 AMO_PANDAS_TYPE_MAPPING = {
     2: 'string',
-    6: 'int64',
-    8: 'float64',
+    6: 'Int64',
+    8: 'Float64',
     9: 'datetime64[ns]',
     10: 'decimal.Decimal',
     11: 'bool',
     17: 'bytes'
 }
 
 # ---------- UTILITY FUNCTIONS ----------
```

### Comparing `pbixray-0.1.13/pbixray/vertipaq_decoder.py` & `pbixray-0.1.14/pbixray/vertipaq_decoder.py`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/pbixray.egg-info/PKG-INFO` & `pbixray-0.1.14/pbixray.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbixray
-Version: 0.1.13
+Version: 0.1.14
 Summary: A Python library to parse and analyze PBIX files used with Microsoft Power BI.
 Home-page: https://github.com/Hugoberry/pbixray
 Author: Igor Cotruta
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -24,25 +24,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: kaitaistruct
 Requires-Dist: pandas
 Requires-Dist: apsw
 
 # PBIXRay
-
+[![Downloads](https://static.pepy.tech/badge/pbixray)](https://pepy.tech/project/pbixray)
 ## Overview
 
 PBIXRay is a Python library designed to parse and analyze PBIX files, which are used with Microsoft Power BI. This library provides a straightforward way to extract valuable information from PBIX files, including tables, metadata, Power Query code, and more.
 
 ## Installation
 
 Before using PBIXRay, ensure you have the following Python modules installed: `apsw`, `kaitaistruct`, and `pbixray`. You can install them using pip:
 
 ```bash
-pip install apsw kaitaistruct pbixray
+pip install pbixray
 ```
 
 ## Getting Started
 To start using PBIXRay, import the module and initialize it with the path to your PBIX file:
 ```python
 from pbixray import PBIXRay
```

### Comparing `pbixray-0.1.13/pbixray.egg-info/SOURCES.txt` & `pbixray-0.1.14/pbixray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pbixray-0.1.13/setup.py` & `pbixray-0.1.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pbixray',
-    version='0.1.13',
+    version='0.1.14',
     packages=find_packages(),
     install_requires=[
         'kaitaistruct',
         'pandas',
         'apsw'
     ],
     include_package_data=True,
```

### Comparing `pbixray-0.1.13/test/test_basic_operation.py` & `pbixray-0.1.14/test/test_basic_operation.py`

 * *Files identical despite different names*

