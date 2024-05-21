# Comparing `tmp/logyca_postgres-0.0.1rc1.tar.gz` & `tmp/logyca_postgres-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logyca_postgres-0.0.1rc1.tar", last modified: Tue May 21 20:00:33 2024, max compression
+gzip compressed data, was "logyca_postgres-0.1.0.tar", last modified: Tue May 21 20:56:23 2024, max compression
```

## Comparing `logyca_postgres-0.0.1rc1.tar` & `logyca_postgres-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 20:00:33.222208 logyca_postgres-0.0.1rc1/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_postgres-0.0.1rc1/LICENSE.txt
--rw-rw-rw-   0        0        0    15494 2024-05-21 20:00:33.221207 logyca_postgres-0.0.1rc1/PKG-INFO
--rw-rw-rw-   0        0        0    12587 2024-05-21 19:42:28.000000 logyca_postgres-0.0.1rc1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 20:00:33.191527 logyca_postgres-0.0.1rc1/logyca_postgres/
--rw-rw-rw-   0        0        0      813 2024-04-26 23:15:08.000000 logyca_postgres-0.0.1rc1/logyca_postgres/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:00:33.207196 logyca_postgres-0.0.1rc1/logyca_postgres/dependencies/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.0.1rc1/logyca_postgres/dependencies/__init__.py
--rw-rw-rw-   0        0        0     9945 2024-04-26 23:13:21.000000 logyca_postgres-0.0.1rc1/logyca_postgres/dependencies/conn_postgres_async.py
--rw-rw-rw-   0        0        0     9988 2024-05-20 21:52:10.000000 logyca_postgres-0.0.1rc1/logyca_postgres/dependencies/conn_postgres_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:00:33.209189 logyca_postgres-0.0.1rc1/logyca_postgres/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.0.1rc1/logyca_postgres/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:00:33.215188 logyca_postgres-0.0.1rc1/logyca_postgres/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.0.1rc1/logyca_postgres/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0      228 2024-04-23 14:32:08.000000 logyca_postgres-0.0.1rc1/logyca_postgres/utils/helpers/functions.py
--rw-rw-rw-   0        0        0      331 2024-04-23 14:32:08.000000 logyca_postgres-0.0.1rc1/logyca_postgres/utils/helpers/singleton.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:00:33.217209 logyca_postgres-0.0.1rc1/logyca_postgres.egg-info/
--rw-rw-rw-   0        0        0    15494 2024-05-21 20:00:33.000000 logyca_postgres-0.0.1rc1/logyca_postgres.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      568 2024-05-21 20:00:33.000000 logyca_postgres-0.0.1rc1/logyca_postgres.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 20:00:33.000000 logyca_postgres-0.0.1rc1/logyca_postgres.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      445 2024-05-21 20:00:33.000000 logyca_postgres-0.0.1rc1/logyca_postgres.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-21 20:00:33.000000 logyca_postgres-0.0.1rc1/logyca_postgres.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 20:00:33.223206 logyca_postgres-0.0.1rc1/setup.cfg
--rw-rw-rw-   0        0        0     2592 2024-05-21 19:50:50.000000 logyca_postgres-0.0.1rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:56:23.069855 logyca_postgres-0.1.0/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_postgres-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    15491 2024-05-21 20:56:23.068855 logyca_postgres-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12587 2024-05-21 19:42:28.000000 logyca_postgres-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 20:56:23.037930 logyca_postgres-0.1.0/logyca_postgres/
+-rw-rw-rw-   0        0        0      813 2024-04-26 23:15:08.000000 logyca_postgres-0.1.0/logyca_postgres/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:56:23.053857 logyca_postgres-0.1.0/logyca_postgres/dependencies/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.0/logyca_postgres/dependencies/__init__.py
+-rw-rw-rw-   0        0        0     9945 2024-04-26 23:13:21.000000 logyca_postgres-0.1.0/logyca_postgres/dependencies/conn_postgres_async.py
+-rw-rw-rw-   0        0        0     9988 2024-05-20 21:52:10.000000 logyca_postgres-0.1.0/logyca_postgres/dependencies/conn_postgres_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:56:23.056858 logyca_postgres-0.1.0/logyca_postgres/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.0/logyca_postgres/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:56:23.062860 logyca_postgres-0.1.0/logyca_postgres/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.0/logyca_postgres/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0      228 2024-04-23 14:32:08.000000 logyca_postgres-0.1.0/logyca_postgres/utils/helpers/functions.py
+-rw-rw-rw-   0        0        0      331 2024-04-23 14:32:08.000000 logyca_postgres-0.1.0/logyca_postgres/utils/helpers/singleton.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:56:23.065859 logyca_postgres-0.1.0/logyca_postgres.egg-info/
+-rw-rw-rw-   0        0        0    15491 2024-05-21 20:56:22.000000 logyca_postgres-0.1.0/logyca_postgres.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2024-05-21 20:56:23.000000 logyca_postgres-0.1.0/logyca_postgres.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 20:56:22.000000 logyca_postgres-0.1.0/logyca_postgres.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      445 2024-05-21 20:56:23.000000 logyca_postgres-0.1.0/logyca_postgres.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-21 20:56:23.000000 logyca_postgres-0.1.0/logyca_postgres.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 20:56:23.071858 logyca_postgres-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2589 2024-05-21 20:54:55.000000 logyca_postgres-0.1.0/setup.py
```

### Comparing `logyca_postgres-0.0.1rc1/LICENSE.txt` & `logyca_postgres-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.0.1rc1/PKG-INFO` & `logyca_postgres-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logyca-postgres
-Version: 0.0.1rc1
+Version: 0.1.0
 Summary: An integration package created by the company LOGYCA that connects Postgres and is used to standardize connections and dependency injection in synchronous or asynchronous mode. Tested in fastapi and in console/worker scripts.
 Home-page: https://github.com/logyca/<soon>
 Author: Jaime Andres Cardona Carrillo
 Author-email: tecnologiaeinformacion@logyca.com
 License: MIT License
 Keywords: postgres,driver database
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logyca-postgres Version: 0.0.1rc1 Summary: An
+Metadata-Version: 2.1 Name: logyca-postgres Version: 0.1.0 Summary: An
 integration package created by the company LOGYCA that connects Postgres and is
 used to standardize connections and dependency injection in synchronous or
 asynchronous mode. Tested in fastapi and in console/worker scripts. Home-page:
 https://github.com/logyca/ Author: Jaime Andres Cardona Carrillo Author-email:
 tecnologiaeinformacion@logyca.com License: MIT License Keywords:
 postgres,driver database Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Information
```

### Comparing `logyca_postgres-0.0.1rc1/README.md` & `logyca_postgres-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.0.1rc1/logyca_postgres/__init__.py` & `logyca_postgres-0.1.0/logyca_postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.0.1rc1/logyca_postgres/dependencies/conn_postgres_async.py` & `logyca_postgres-0.1.0/logyca_postgres/dependencies/conn_postgres_async.py`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.0.1rc1/logyca_postgres/dependencies/conn_postgres_sync.py` & `logyca_postgres-0.1.0/logyca_postgres/dependencies/conn_postgres_sync.py`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.0.1rc1/logyca_postgres.egg-info/PKG-INFO` & `logyca_postgres-0.1.0/logyca_postgres.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logyca-postgres
-Version: 0.0.1rc1
+Version: 0.1.0
 Summary: An integration package created by the company LOGYCA that connects Postgres and is used to standardize connections and dependency injection in synchronous or asynchronous mode. Tested in fastapi and in console/worker scripts.
 Home-page: https://github.com/logyca/<soon>
 Author: Jaime Andres Cardona Carrillo
 Author-email: tecnologiaeinformacion@logyca.com
 License: MIT License
 Keywords: postgres,driver database
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logyca-postgres Version: 0.0.1rc1 Summary: An
+Metadata-Version: 2.1 Name: logyca-postgres Version: 0.1.0 Summary: An
 integration package created by the company LOGYCA that connects Postgres and is
 used to standardize connections and dependency injection in synchronous or
 asynchronous mode. Tested in fastapi and in console/worker scripts. Home-page:
 https://github.com/logyca/ Author: Jaime Andres Cardona Carrillo Author-email:
 tecnologiaeinformacion@logyca.com License: MIT License Keywords:
 postgres,driver database Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Information
```

### Comparing `logyca_postgres-0.0.1rc1/logyca_postgres.egg-info/SOURCES.txt` & `logyca_postgres-0.1.0/logyca_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.0.1rc1/setup.py` & `logyca_postgres-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="LOGYCA"
 PACKAGE_NAME = "logyca-postgres"
-VERSION = "0.0.1rc1"
+VERSION = "0.1.0"
 
 install_requires = ["SQLAlchemy>=2.0.6","starlette>=0.24.0"]
 install_requires_asyncpg = ["asyncpg >=0.27.0"]
 install_requires_psycopg2 = ["psycopg2 >=2.9.6"]
 install_requires_psycopg2_binary = ["psycopg2-binary >=2.9.6"]
 
 extras_require = {
```

