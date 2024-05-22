# Comparing `tmp/djangondor-1.3.0.tar.gz` & `tmp/djangondor-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangondor-1.3.0.tar", last modified: Fri Oct 13 07:13:16 2023, max compression
+gzip compressed data, was "djangondor-1.3.2.tar", last modified: Wed May 22 18:17:00 2024, max compression
```

## Comparing `djangondor-1.3.0.tar` & `djangondor-1.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-10-13 07:13:16.452092 djangondor-1.3.0/
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1103 2023-10-11 08:50:52.000000 djangondor-1.3.0/LICENSE
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1261 2023-10-13 07:13:16.452092 djangondor-1.3.0/PKG-INFO
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)      349 2023-10-11 08:50:52.000000 djangondor-1.3.0/README.rst
-drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-10-13 07:13:16.442092 djangondor-1.3.0/djangondor/
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)        0 2023-10-11 08:50:52.000000 djangondor-1.3.0/djangondor/__init__.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)       63 2023-10-11 08:50:52.000000 djangondor-1.3.0/djangondor/admin.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)      152 2023-10-11 08:50:52.000000 djangondor-1.3.0/djangondor/apps.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1251 2023-10-11 08:55:34.000000 djangondor-1.3.0/djangondor/collections.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1537 2023-10-11 08:56:49.000000 djangondor-1.3.0/djangondor/models.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)     3417 2023-10-11 08:50:52.000000 djangondor-1.3.0/djangondor/processing.py
-drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-10-13 07:13:16.452092 djangondor-1.3.0/djangondor/templatetags/
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)        0 2023-10-11 08:50:52.000000 djangondor-1.3.0/djangondor/templatetags/__init__.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)      410 2023-10-11 08:50:52.000000 djangondor-1.3.0/djangondor/templatetags/djangondor_collection_tags.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1601 2023-10-11 08:50:52.000000 djangondor-1.3.0/djangondor/templatetags/djangondor_path_tags.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)       60 2023-10-11 08:50:52.000000 djangondor-1.3.0/djangondor/tests.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)      909 2023-10-11 08:50:52.000000 djangondor-1.3.0/djangondor/time.py
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)       63 2023-10-11 08:50:52.000000 djangondor-1.3.0/djangondor/views.py
-drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-10-13 07:13:16.442092 djangondor-1.3.0/djangondor.egg-info/
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1261 2023-10-13 07:13:16.000000 djangondor-1.3.0/djangondor.egg-info/PKG-INFO
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)      552 2023-10-13 07:13:16.000000 djangondor-1.3.0/djangondor.egg-info/SOURCES.txt
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)        1 2023-10-13 07:13:16.000000 djangondor-1.3.0/djangondor.egg-info/dependency_links.txt
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)       12 2023-10-13 07:13:16.000000 djangondor-1.3.0/djangondor.egg-info/requires.txt
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)       11 2023-10-13 07:13:16.000000 djangondor-1.3.0/djangondor.egg-info/top_level.txt
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)       89 2023-10-11 08:50:52.000000 djangondor-1.3.0/pyproject.toml
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)      894 2023-10-13 07:13:16.452092 djangondor-1.3.0/setup.cfg
--rw-r--r--   0 dalitso   (1000) dalitso   (1000)      106 2023-10-11 08:50:52.000000 djangondor-1.3.0/setup.py
+drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2024-05-22 18:17:00.606989 djangondor-1.3.2/
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1103 2023-10-14 14:58:56.000000 djangondor-1.3.2/LICENSE
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1348 2024-05-22 18:17:00.606989 djangondor-1.3.2/PKG-INFO
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)      349 2023-10-14 14:58:56.000000 djangondor-1.3.2/README.rst
+drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2024-05-22 18:17:00.606989 djangondor-1.3.2/djangondor/
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)        0 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/__init__.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)       63 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/admin.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)      152 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/apps.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1251 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/collections.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1636 2023-10-21 16:21:10.000000 djangondor-1.3.2/djangondor/models.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)     3417 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/processing.py
+drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2024-05-22 18:17:00.606989 djangondor-1.3.2/djangondor/templatetags/
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)        0 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/templatetags/__init__.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)      410 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/templatetags/djangondor_collection_tags.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1601 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/templatetags/djangondor_path_tags.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)       60 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/tests.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)      909 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/time.py
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)       63 2023-10-14 14:58:56.000000 djangondor-1.3.2/djangondor/views.py
+drwxr-xr-x   0 dalitso   (1000) dalitso   (1000)        0 2024-05-22 18:17:00.606989 djangondor-1.3.2/djangondor.egg-info/
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)     1348 2024-05-22 18:17:00.000000 djangondor-1.3.2/djangondor.egg-info/PKG-INFO
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)      552 2024-05-22 18:17:00.000000 djangondor-1.3.2/djangondor.egg-info/SOURCES.txt
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)        1 2024-05-22 18:17:00.000000 djangondor-1.3.2/djangondor.egg-info/dependency_links.txt
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)       54 2024-05-22 18:17:00.000000 djangondor-1.3.2/djangondor.egg-info/requires.txt
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)       11 2024-05-22 18:17:00.000000 djangondor-1.3.2/djangondor.egg-info/top_level.txt
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)       89 2023-10-14 14:58:56.000000 djangondor-1.3.2/pyproject.toml
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)      945 2024-05-22 18:17:00.606989 djangondor-1.3.2/setup.cfg
+-rw-r--r--   0 dalitso   (1000) dalitso   (1000)      106 2023-10-14 14:58:56.000000 djangondor-1.3.2/setup.py
```

### Comparing `djangondor-1.3.0/LICENSE` & `djangondor-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djangondor-1.3.0/PKG-INFO` & `djangondor-1.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangondor
-Version: 1.3.0
+Version: 1.3.2
 Summary: A collection of django utilities.
 Home-page: https://github.com/dalitsosakala/djangondor
 Author: Dalitso Sakala
 Author-email: dalitso.1sc@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -18,14 +18,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Django>=4.2
+Requires-Dist: openpyxl>=3.1
+Requires-Dist: pandas>=2.1
+Requires-Dist: XlsxWriter>=3.1
 
 ==========
 Djangondor
 ==========
 
 Djangondor is a collection Django utilities.
```

### Comparing `djangondor-1.3.0/djangondor/collections.py` & `djangondor-1.3.2/djangondor/collections.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.3.0/djangondor/models.py` & `djangondor-1.3.2/djangondor/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 # NULLABLE
 # USAGE
 # =====
 # description = models.CharField(max_length=200,**NULLABLE)
 # # is the same as:
 # description = models.CharField(max_length=200,null=True,default=None,blank=True)
 NULLABLE = {"null": True, "default": None, "blank": True}
-NULLABLE_CHARFIELD = {**NULLABLE, "max_length": 100}
+NULLABLE_CHARFIELD = {**NULLABLE, "max_length": 250}
+NON_NULL_BLANK_CHARFIELD = {"blank":True, "max_length": 225}
 
 
 # UUID_PK
 # USAGE
 # =====
 # id=models.UUIDField(**UUID_PK)
 # # is the same as:
@@ -25,14 +26,16 @@
 
 def make_choices(*entries):
     """Make choices to passed to model field `choices` attribute. Each entry has the form `(entry,entry)`"""
     return [(value, value) for value in entries]
 
 def check_if_tables_exist(*table_names: str):
     '''Check if tables exist in the database'''
+    from django.db import connection
+
     all_tables = connection.introspection.table_names()
     tables = set(table_names)
     return len(tables.intersection(all_tables)) == len(tables)
 
 class BaseTimestampModel(models.Model):
     """Inherit this model to add time stamps to your models"""
```

### Comparing `djangondor-1.3.0/djangondor/processing.py` & `djangondor-1.3.2/djangondor/processing.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.3.0/djangondor/templatetags/djangondor_path_tags.py` & `djangondor-1.3.2/djangondor/templatetags/djangondor_path_tags.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.3.0/djangondor/time.py` & `djangondor-1.3.2/djangondor/time.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.3.0/djangondor.egg-info/PKG-INFO` & `djangondor-1.3.2/djangondor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangondor
-Version: 1.3.0
+Version: 1.3.2
 Summary: A collection of django utilities.
 Home-page: https://github.com/dalitsosakala/djangondor
 Author: Dalitso Sakala
 Author-email: dalitso.1sc@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -18,14 +18,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Django>=4.2
+Requires-Dist: openpyxl>=3.1
+Requires-Dist: pandas>=2.1
+Requires-Dist: XlsxWriter>=3.1
 
 ==========
 Djangondor
 ==========
 
 Djangondor is a collection Django utilities.
```

### Comparing `djangondor-1.3.0/djangondor.egg-info/SOURCES.txt` & `djangondor-1.3.2/djangondor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangondor-1.3.0/setup.cfg` & `djangondor-1.3.2/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangondor
-version = 1.3.0
+version = 1.3.2
 description = A collection of django utilities.
 long_description = file: README.rst
 url = https://github.com/dalitsosakala/djangondor
 author = Dalitso Sakala
 author_email = dalitso.1sc@gmail.com
 license = MIT License
 classifiers = 
@@ -24,12 +24,15 @@
 
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	Django >= 4.2
+	openpyxl >= 3.1
+	pandas >= 2.1
+	XlsxWriter >= 3.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

