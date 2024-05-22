# Comparing `tmp/stimulsoft_data_adapters-2024.2.5.tar.gz` & `tmp/stimulsoft_data_adapters-2024.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stimulsoft_data_adapters-2024.2.5.tar", last modified: Wed May  8 10:57:59 2024, max compression
+gzip compressed data, was "stimulsoft_data_adapters-2024.2.6.tar", last modified: Mon May 20 14:21:09 2024, max compression
```

## Comparing `stimulsoft_data_adapters-2024.2.5.tar` & `stimulsoft_data_adapters-2024.2.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 10:57:59.226661 stimulsoft_data_adapters-2024.2.5/
--rw-rw-rw-   0        0        0    25131 2024-02-19 11:37:32.000000 stimulsoft_data_adapters-2024.2.5/LICENSE.md
--rw-rw-rw-   0        0        0     9937 2024-05-08 10:57:59.225660 stimulsoft_data_adapters-2024.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     9130 2024-03-07 13:34:04.000000 stimulsoft_data_adapters-2024.2.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 10:57:59.226661 stimulsoft_data_adapters-2024.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1209 2024-05-08 10:57:58.000000 stimulsoft_data_adapters-2024.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:57:59.217661 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/
--rw-rw-rw-   0        0        0     8777 2024-05-08 10:55:36.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiDataAdapter.py
--rw-rw-rw-   0        0        0     2153 2024-05-08 10:57:58.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiFirebirdAdapter.py
--rw-rw-rw-   0        0        0     4725 2024-05-08 10:57:58.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiMongoDbAdapter.py
--rw-rw-rw-   0        0        0     3805 2024-05-08 10:57:58.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiMsSqlAdapter.py
--rw-rw-rw-   0        0        0     3087 2024-05-08 10:57:58.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiMySqlAdapter.py
--rw-rw-rw-   0        0        0     1124 2024-05-08 10:57:58.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiOdbcAdapter.py
--rw-rw-rw-   0        0        0     4247 2024-05-08 10:57:58.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiOracleAdapter.py
--rw-rw-rw-   0        0        0     2735 2024-05-08 10:57:58.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiPostgreSqlAdapter.py
--rw-rw-rw-   0        0        0      204 2023-11-14 15:52:08.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:57:59.222660 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/classes/
--rw-rw-rw-   0        0        0     9170 2024-05-08 10:57:58.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/classes/StiBaseHandler.py
--rw-rw-rw-   0        0        0     2102 2024-05-08 09:22:23.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/classes/StiBaseRequest.py
--rw-rw-rw-   0        0        0     3454 2024-05-08 10:55:36.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/classes/StiBaseResponse.py
--rw-rw-rw-   0        0        0      883 2024-05-08 10:55:36.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/classes/StiBaseResult.py
--rw-rw-rw-   0        0        0      336 2023-09-22 14:50:49.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/classes/StiConnectionInfo.py
--rw-rw-rw-   0        0        0     1368 2024-05-08 10:55:36.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/classes/StiDataResult.py
--rw-rw-rw-   0        0        0      786 2023-10-30 12:49:14.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/classes/StiParameter.py
--rw-rw-rw-   0        0        0        0 2023-09-29 07:52:43.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/classes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:57:59.224660 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/enums/
--rw-rw-rw-   0        0        0      282 2024-05-08 10:55:36.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/enums/StiDataCommand.py
--rw-rw-rw-   0        0        0      456 2024-05-08 10:55:36.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/enums/StiDatabaseType.py
--rw-rw-rw-   0        0        0      175 2023-10-30 08:59:56.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/enums/StiFrameworkType.py
--rw-rw-rw-   0        0        0       88 2023-11-16 09:48:40.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:57:59.225660 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/events/
--rw-rw-rw-   0        0        0     1074 2023-10-30 12:47:41.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/events/StiDataEventArgs.py
--rw-rw-rw-   0        0        0     1651 2024-05-08 10:55:36.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/events/StiEvent.py
--rw-rw-rw-   0        0        0      585 2024-05-06 14:56:11.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/events/StiEventArgs.py
--rw-rw-rw-   0        0        0       46 2023-11-14 15:52:07.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/events/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:57:59.219661 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters.egg-info/
--rw-rw-rw-   0        0        0     9937 2024-05-08 10:57:59.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1449 2024-05-08 10:57:59.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 10:57:59.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2024-05-08 10:57:59.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-05-08 10:57:59.000000 stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 14:21:09.478722 stimulsoft_data_adapters-2024.2.6/
+-rw-rw-rw-   0        0        0    25131 2024-02-19 11:37:32.000000 stimulsoft_data_adapters-2024.2.6/LICENSE.md
+-rw-rw-rw-   0        0        0     9937 2024-05-20 14:21:09.478722 stimulsoft_data_adapters-2024.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9130 2024-03-07 13:34:04.000000 stimulsoft_data_adapters-2024.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-20 14:21:09.478722 stimulsoft_data_adapters-2024.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2024-05-20 14:06:36.000000 stimulsoft_data_adapters-2024.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:21:09.470722 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/
+-rw-rw-rw-   0        0        0     8777 2024-05-20 14:06:10.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiDataAdapter.py
+-rw-rw-rw-   0        0        0     2153 2024-05-20 14:06:36.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiFirebirdAdapter.py
+-rw-rw-rw-   0        0        0     4725 2024-05-20 14:06:36.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiMongoDbAdapter.py
+-rw-rw-rw-   0        0        0     3805 2024-05-20 14:06:36.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiMsSqlAdapter.py
+-rw-rw-rw-   0        0        0     3087 2024-05-20 14:06:36.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiMySqlAdapter.py
+-rw-rw-rw-   0        0        0     1124 2024-05-20 14:06:36.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiOdbcAdapter.py
+-rw-rw-rw-   0        0        0     4247 2024-05-20 14:06:36.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiOracleAdapter.py
+-rw-rw-rw-   0        0        0     2735 2024-05-20 14:06:36.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiPostgreSqlAdapter.py
+-rw-rw-rw-   0        0        0      204 2023-11-14 15:52:08.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:21:09.475723 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/classes/
+-rw-rw-rw-   0        0        0     9170 2024-05-20 14:06:36.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/classes/StiBaseHandler.py
+-rw-rw-rw-   0        0        0     2102 2024-05-08 09:22:23.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/classes/StiBaseRequest.py
+-rw-rw-rw-   0        0        0     3454 2024-05-20 14:06:10.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/classes/StiBaseResponse.py
+-rw-rw-rw-   0        0        0      883 2024-05-20 14:06:10.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/classes/StiBaseResult.py
+-rw-rw-rw-   0        0        0      336 2023-09-22 14:50:49.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/classes/StiConnectionInfo.py
+-rw-rw-rw-   0        0        0     1368 2024-05-20 14:06:10.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/classes/StiDataResult.py
+-rw-rw-rw-   0        0        0      786 2023-10-30 12:49:14.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/classes/StiParameter.py
+-rw-rw-rw-   0        0        0        0 2023-09-29 07:52:43.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/classes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:21:09.476722 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/enums/
+-rw-rw-rw-   0        0        0      282 2024-05-20 14:06:10.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/enums/StiDataCommand.py
+-rw-rw-rw-   0        0        0      456 2024-05-20 14:06:10.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/enums/StiDatabaseType.py
+-rw-rw-rw-   0        0        0      175 2023-10-30 08:59:56.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/enums/StiFrameworkType.py
+-rw-rw-rw-   0        0        0       88 2023-11-16 09:48:40.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:21:09.477722 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/events/
+-rw-rw-rw-   0        0        0     1074 2023-10-30 12:47:41.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/events/StiDataEventArgs.py
+-rw-rw-rw-   0        0        0     1651 2024-05-20 14:06:10.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/events/StiEvent.py
+-rw-rw-rw-   0        0        0      585 2024-05-06 14:56:11.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/events/StiEventArgs.py
+-rw-rw-rw-   0        0        0       46 2023-11-14 15:52:07.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/events/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:21:09.472722 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters.egg-info/
+-rw-rw-rw-   0        0        0     9937 2024-05-20 14:21:09.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1449 2024-05-20 14:21:09.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 14:21:09.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2024-05-20 14:21:09.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-20 14:21:09.000000 stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters.egg-info/top_level.txt
```

### Comparing `stimulsoft_data_adapters-2024.2.5/LICENSE.md` & `stimulsoft_data_adapters-2024.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.5/PKG-INFO` & `stimulsoft_data_adapters-2024.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimulsoft_data_adapters
-Version: 2024.2.5
+Version: 2024.2.6
 Summary: Stimulsoft data adapters for Python.
 Home-page: https://www.stimulsoft.com/en/products/reports-python
 Author: Stimulsoft
 Author-email: info@stimulsoft.com
 License: https://www.stimulsoft.com/en/licensing/developers
 Classifier: License :: Other/Proprietary License
 Classifier: Framework :: Django
```

### Comparing `stimulsoft_data_adapters-2024.2.5/README.md` & `stimulsoft_data_adapters-2024.2.6/README.md`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.5/setup.py` & `stimulsoft_data_adapters-2024.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readmeFile = file.read()
 
 with open('REQUIREMENTS.txt') as file:
     requiresFile = [text.strip() for text in file if text.strip()]
 
 setup(
     name = 'stimulsoft_data_adapters',
-    version = '2024.2.5',
+    version = '2024.2.6',
     author = 'Stimulsoft',
     author_email = 'info@stimulsoft.com',
     description = 'Stimulsoft data adapters for Python.',
     long_description = readmeFile,
     long_description_content_type = 'text/markdown',
     url = 'https://www.stimulsoft.com/en/products/reports-python',
     license = 'https://www.stimulsoft.com/en/licensing/developers',
```

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiDataAdapter.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiDataAdapter.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiFirebirdAdapter.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiFirebirdAdapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .classes.StiDataResult import StiDataResult
 from .StiDataAdapter import StiDataAdapter
 
 
 class StiFirebirdAdapter(StiDataAdapter):
-    version: str = '2024.2.5'
+    version: str = '2024.2.6'
     checkVersion: bool = True
 
     def getOdbcConnectionString(self):
         connectionString: str = \
             f'Driver={self.connectionInfo.driver};' \
             f'Dbname={self.connectionInfo.host}/{self.connectionInfo.port}:{self.connectionInfo.database};' \
             f'Uid={self.connectionInfo.userId};' \
```

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiMongoDbAdapter.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiMongoDbAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from urllib.parse import urlparse
 
 from .classes.StiDataResult import StiDataResult
 from .StiDataAdapter import StiDataAdapter
 
 
 class StiMongoDbAdapter(StiDataAdapter):
-    version: str = '2024.2.5'
+    version: str = '2024.2.6'
     checkVersion: bool = True
 
     def connect(self):
         try:
             from pymongo import MongoClient
             self.connectionLink = MongoClient(self.connectionString)
         except Exception as e:
```

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiMsSqlAdapter.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiMsSqlAdapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from uuid import UUID
 
 from .classes.StiDataResult import StiDataResult
 from .StiDataAdapter import StiDataAdapter
 
 
 class StiMsSqlAdapter(StiDataAdapter):
-    version: str = '2024.2.5'
+    version: str = '2024.2.6'
     checkVersion: bool = True
     trustServerCertificate: str = None
     integratedSecurity: str = None
 
     def getOdbcConnectionString(self):
         connectionString: str = \
             f'Driver={self.connectionInfo.driver};' \
```

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiMySqlAdapter.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiMySqlAdapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .classes.StiDataResult import StiDataResult
 from .classes.StiBaseResult import StiBaseResult
 from .StiDataAdapter import StiDataAdapter
 
 
 class StiMySqlAdapter(StiDataAdapter):
-    version: str = '2024.2.5'
+    version: str = '2024.2.6'
     checkVersion: bool = True
     
     def connect(self):
         if self.connectionInfo.driver:
             return self.connectOdbc()
         
         if not self.connectionInfo.charset:
```

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiOdbcAdapter.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiOdbcAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pyodbc import Connection
 
 from .classes.StiDataResult import StiDataResult
 from .StiDataAdapter import StiDataAdapter
 
 
 class StiOdbcAdapter(StiDataAdapter):
-    version: str = '2024.2.5'
+    version: str = '2024.2.6'
     checkVersion: bool = True
     connectionLink: Connection
 
     def connect(self):
         try:
             self.connectionLink = pyodbc.connect(self.connectionString)
             if self.connectionInfo.charset:
```

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiOracleAdapter.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiOracleAdapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .classes.StiDataResult import StiDataResult
 from .StiDataAdapter import StiDataAdapter
 
 
 class StiOracleAdapter(StiDataAdapter):
-    version: str = '2024.2.5'
+    version: str = '2024.2.6'
     checkVersion: bool = True
 
     def getOdbcConnectionString(self):
         connectionString: str = \
             f'Driver={self.connectionInfo.driver};' \
             f'Dbq={self.connectionInfo.database};' \
             f'Uid={self.connectionInfo.userId};' \
```

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/StiPostgreSqlAdapter.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/StiPostgreSqlAdapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .classes.StiDataResult import StiDataResult
 from .StiDataAdapter import StiDataAdapter
 
 
 class StiPostgreSqlAdapter(StiDataAdapter):
-    version: str = '2024.2.5'
+    version: str = '2024.2.6'
     checkVersion: bool = True
 
     def connect(self):
         if self.connectionInfo.driver:
             return self.connectOdbc()
         
         if not self.connectionInfo.charset:
```

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/classes/StiBaseHandler.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/classes/StiBaseHandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class StiBaseHandler:
     """
     Event handler for all requests from the report generator. 
     The incoming request is processed, a data adapter is created and all necessary actions are performed.
     """
 
-    version: str = '2024.2.5'
+    version: str = '2024.2.6'
     checkDataAdaptersVersion: bool = True
     framework: str = StiFrameworkType.DEFAULT
     origin: str = None
     query: dict = None
     body: str = None
     error: str = None
     request: StiBaseRequest = None
```

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/classes/StiBaseRequest.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/classes/StiBaseRequest.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/classes/StiBaseResponse.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/classes/StiBaseResponse.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/classes/StiBaseResult.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/classes/StiBaseResult.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/classes/StiDataResult.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/classes/StiDataResult.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/classes/StiParameter.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/classes/StiParameter.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/events/StiDataEventArgs.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/events/StiDataEventArgs.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/events/StiEvent.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/events/StiEvent.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters/events/StiEventArgs.py` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters/events/StiEventArgs.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters.egg-info/PKG-INFO` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimulsoft-data-adapters
-Version: 2024.2.5
+Version: 2024.2.6
 Summary: Stimulsoft data adapters for Python.
 Home-page: https://www.stimulsoft.com/en/products/reports-python
 Author: Stimulsoft
 Author-email: info@stimulsoft.com
 License: https://www.stimulsoft.com/en/licensing/developers
 Classifier: License :: Other/Proprietary License
 Classifier: Framework :: Django
```

### Comparing `stimulsoft_data_adapters-2024.2.5/stimulsoft_data_adapters.egg-info/SOURCES.txt` & `stimulsoft_data_adapters-2024.2.6/stimulsoft_data_adapters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

