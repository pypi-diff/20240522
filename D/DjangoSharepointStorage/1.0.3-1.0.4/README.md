# Comparing `tmp/DjangoSharepointStorage-1.0.3.tar.gz` & `tmp/DjangoSharepointStorage-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DjangoSharepointStorage-1.0.3.tar", last modified: Tue May 21 23:13:25 2024, max compression
+gzip compressed data, was "DjangoSharepointStorage-1.0.4.tar", last modified: Wed May 22 08:28:31 2024, max compression
```

## Comparing `DjangoSharepointStorage-1.0.3.tar` & `DjangoSharepointStorage-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2024-05-21 23:13:25.895666 DjangoSharepointStorage-1.0.3/
-drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2024-05-21 23:13:25.895299 DjangoSharepointStorage-1.0.3/DjangoSharepointStorage.egg-info/
--rw-r--r--   0 melihsunbul   (501) staff       (20)      613 2024-05-21 23:13:25.000000 DjangoSharepointStorage-1.0.3/DjangoSharepointStorage.egg-info/PKG-INFO
--rw-r--r--   0 melihsunbul   (501) staff       (20)      497 2024-05-21 23:13:25.000000 DjangoSharepointStorage-1.0.3/DjangoSharepointStorage.egg-info/SOURCES.txt
--rw-r--r--   0 melihsunbul   (501) staff       (20)        1 2024-05-21 23:13:25.000000 DjangoSharepointStorage-1.0.3/DjangoSharepointStorage.egg-info/dependency_links.txt
--rw-r--r--   0 melihsunbul   (501) staff       (20)       36 2024-05-21 23:13:25.000000 DjangoSharepointStorage-1.0.3/DjangoSharepointStorage.egg-info/requires.txt
--rw-r--r--   0 melihsunbul   (501) staff       (20)       26 2024-05-21 23:13:25.000000 DjangoSharepointStorage-1.0.3/DjangoSharepointStorage.egg-info/top_level.txt
--rw-r--r--   0 melihsunbul   (501) staff       (20)     1071 2023-11-09 16:23:47.000000 DjangoSharepointStorage-1.0.3/LICENSE.txt
--rw-r--r--   0 melihsunbul   (501) staff       (20)      613 2024-05-21 23:13:25.895484 DjangoSharepointStorage-1.0.3/PKG-INFO
--rw-r--r--   0 melihsunbul   (501) staff       (20)       34 2024-05-21 07:57:25.000000 DjangoSharepointStorage-1.0.3/README.md
-drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2024-05-21 23:13:25.895147 DjangoSharepointStorage-1.0.3/django_sharepoint_storage/
--rw-r--r--   0 melihsunbul   (501) staff       (20)      493 2023-11-21 10:32:47.000000 DjangoSharepointStorage-1.0.3/django_sharepoint_storage/SharePointClients.py
--rw-r--r--   0 melihsunbul   (501) staff       (20)      592 2023-11-21 10:32:47.000000 DjangoSharepointStorage-1.0.3/django_sharepoint_storage/SharePointCloudStorageUtils.py
--rw-r--r--   0 melihsunbul   (501) staff       (20)      735 2023-11-16 09:06:38.000000 DjangoSharepointStorage-1.0.3/django_sharepoint_storage/SharePointFile.py
--rw-r--r--   0 melihsunbul   (501) staff       (20)     4780 2024-05-21 23:12:37.000000 DjangoSharepointStorage-1.0.3/django_sharepoint_storage/SharePointStorage.py
--rw-r--r--   0 melihsunbul   (501) staff       (20)        0 2023-10-30 10:29:18.000000 DjangoSharepointStorage-1.0.3/django_sharepoint_storage/__init__.py
--rw-r--r--   0 melihsunbul   (501) staff       (20)       38 2024-05-21 23:13:25.895711 DjangoSharepointStorage-1.0.3/setup.cfg
--rw-r--r--   0 melihsunbul   (501) staff       (20)      853 2024-05-21 23:12:37.000000 DjangoSharepointStorage-1.0.3/setup.py
+drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2024-05-22 08:28:31.517676 DjangoSharepointStorage-1.0.4/
+drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2024-05-22 08:28:31.517340 DjangoSharepointStorage-1.0.4/DjangoSharepointStorage.egg-info/
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      613 2024-05-22 08:28:31.000000 DjangoSharepointStorage-1.0.4/DjangoSharepointStorage.egg-info/PKG-INFO
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      497 2024-05-22 08:28:31.000000 DjangoSharepointStorage-1.0.4/DjangoSharepointStorage.egg-info/SOURCES.txt
+-rw-r--r--   0 melihsunbul   (501) staff       (20)        1 2024-05-22 08:28:31.000000 DjangoSharepointStorage-1.0.4/DjangoSharepointStorage.egg-info/dependency_links.txt
+-rw-r--r--   0 melihsunbul   (501) staff       (20)       36 2024-05-22 08:28:31.000000 DjangoSharepointStorage-1.0.4/DjangoSharepointStorage.egg-info/requires.txt
+-rw-r--r--   0 melihsunbul   (501) staff       (20)       26 2024-05-22 08:28:31.000000 DjangoSharepointStorage-1.0.4/DjangoSharepointStorage.egg-info/top_level.txt
+-rw-r--r--   0 melihsunbul   (501) staff       (20)     1071 2023-11-09 16:23:47.000000 DjangoSharepointStorage-1.0.4/LICENSE.txt
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      613 2024-05-22 08:28:31.517509 DjangoSharepointStorage-1.0.4/PKG-INFO
+-rw-r--r--   0 melihsunbul   (501) staff       (20)       34 2024-05-21 07:57:25.000000 DjangoSharepointStorage-1.0.4/README.md
+drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2024-05-22 08:28:31.517202 DjangoSharepointStorage-1.0.4/django_sharepoint_storage/
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      493 2023-11-21 10:32:47.000000 DjangoSharepointStorage-1.0.4/django_sharepoint_storage/SharePointClients.py
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      592 2023-11-21 10:32:47.000000 DjangoSharepointStorage-1.0.4/django_sharepoint_storage/SharePointCloudStorageUtils.py
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      735 2023-11-16 09:06:38.000000 DjangoSharepointStorage-1.0.4/django_sharepoint_storage/SharePointFile.py
+-rw-r--r--   0 melihsunbul   (501) staff       (20)     5167 2024-05-22 08:28:23.000000 DjangoSharepointStorage-1.0.4/django_sharepoint_storage/SharePointStorage.py
+-rw-r--r--   0 melihsunbul   (501) staff       (20)        0 2023-10-30 10:29:18.000000 DjangoSharepointStorage-1.0.4/django_sharepoint_storage/__init__.py
+-rw-r--r--   0 melihsunbul   (501) staff       (20)       38 2024-05-22 08:28:31.517724 DjangoSharepointStorage-1.0.4/setup.cfg
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      853 2024-05-22 08:28:23.000000 DjangoSharepointStorage-1.0.4/setup.py
```

### Comparing `DjangoSharepointStorage-1.0.3/DjangoSharepointStorage.egg-info/PKG-INFO` & `DjangoSharepointStorage-1.0.4/DjangoSharepointStorage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DjangoSharepointStorage
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python library to use SharePoint as storage backend for your Django application
 Home-page: https://github.com/LundIT/DjangoSharepointStorage
 Author: Melih Sünbül
 Author-email: m.sunbul@lund-it.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DjangoSharepointStorage-1.0.3/LICENSE.txt` & `DjangoSharepointStorage-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DjangoSharepointStorage-1.0.3/PKG-INFO` & `DjangoSharepointStorage-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DjangoSharepointStorage
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python library to use SharePoint as storage backend for your Django application
 Home-page: https://github.com/LundIT/DjangoSharepointStorage
 Author: Melih Sünbül
 Author-email: m.sunbul@lund-it.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DjangoSharepointStorage-1.0.3/django_sharepoint_storage/SharePointCloudStorageUtils.py` & `DjangoSharepointStorage-1.0.4/django_sharepoint_storage/SharePointCloudStorageUtils.py`

 * *Files identical despite different names*

### Comparing `DjangoSharepointStorage-1.0.3/django_sharepoint_storage/SharePointFile.py` & `DjangoSharepointStorage-1.0.4/django_sharepoint_storage/SharePointFile.py`

 * *Files identical despite different names*

### Comparing `DjangoSharepointStorage-1.0.3/django_sharepoint_storage/SharePointStorage.py` & `DjangoSharepointStorage-1.0.4/django_sharepoint_storage/SharePointStorage.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,22 @@
         file_content = content.read()
 
         target_folder.upload_file(os.path.basename(name), file_content).execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
 
         return name
 
     def delete(self, name):
-        file = File.from_url(self.url(name)).with_credentials(client_credentials).execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
-        file.delete_object().execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
+        from django_sharepoint_storage.SharePointCloudStorageUtils import get_server_relative_path
+
+        file_path = get_server_relative_path(self.url(name))
+        file = ctx.web.get_file_by_server_relative_path(file_path).get().execute_query_retry(max_retry=5,
+                                                                                             timeout_secs=5,
+                                                                                             failure_callback=SharePointStorage.print_failure)
+        file.delete_object().execute_query_retry(max_retry=5, timeout_secs=5,
+                                                 failure_callback=SharePointStorage.print_failure)
 
     def exists(self, name, retries=5):
         from django_sharepoint_storage.SharePointCloudStorageUtils import get_server_relative_path
 
         file_path = get_server_relative_path(self.url(name))
 
         if retries <= 0:
```

### Comparing `DjangoSharepointStorage-1.0.3/setup.py` & `DjangoSharepointStorage-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="DjangoSharepointStorage",
-    version="1.0.3",
+    version="1.0.4",
     author="Melih Sünbül",
     author_email="m.sunbul@lund-it.com",
     description="A Python library to use SharePoint as storage backend for your Django application",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LundIT/DjangoSharepointStorage",
     packages=find_packages(),
```

