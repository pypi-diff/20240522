# Comparing `tmp/dbcls-1.0.6.tar.gz` & `tmp/dbcls-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbcls-1.0.6.tar", last modified: Tue Jan  9 13:05:19 2024, max compression
+gzip compressed data, was "dbcls-1.0.7.tar", last modified: Wed May 22 07:41:58 2024, max compression
```

## Comparing `dbcls-1.0.6.tar` & `dbcls-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-01-09 13:05:19.949589 dbcls-1.0.6/
--rw-r--r--   0 user       (501) staff       (20)     1492 2023-08-26 08:16:50.000000 dbcls-1.0.6/LICENSE
--rw-r--r--   0 user       (501) staff       (20)       25 2023-08-26 18:36:21.000000 dbcls-1.0.6/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     1637 2024-01-09 13:05:19.949302 dbcls-1.0.6/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     1123 2023-08-26 19:12:56.000000 dbcls-1.0.6/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-01-09 13:05:19.945634 dbcls-1.0.6/dbcls/
--rw-r--r--   0 user       (501) staff       (20)       24 2023-08-26 18:47:19.000000 dbcls-1.0.6/dbcls/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-01-09 13:05:19.948360 dbcls-1.0.6/dbcls/clients/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-08-26 13:23:14.000000 dbcls-1.0.6/dbcls/clients/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1405 2023-10-17 05:51:47.000000 dbcls-1.0.6/dbcls/clients/base.py
--rw-r--r--   0 user       (501) staff       (20)     1361 2024-01-09 12:58:02.000000 dbcls-1.0.6/dbcls/clients/clickhouse.py
--rw-r--r--   0 user       (501) staff       (20)     1143 2023-12-20 10:05:53.000000 dbcls-1.0.6/dbcls/clients/mysql.py
--rw-r--r--   0 user       (501) staff       (20)     2027 2023-10-17 05:51:47.000000 dbcls-1.0.6/dbcls/clients/postgres.py
--rw-r--r--   0 user       (501) staff       (20)     1407 2023-12-20 10:29:15.000000 dbcls-1.0.6/dbcls/clients/sqlite3.py
--rw-r--r--   0 user       (501) staff       (20)    11641 2023-12-20 13:43:21.000000 dbcls-1.0.6/dbcls/dbcls.py
--rw-r--r--   0 user       (501) staff       (20)     1826 2023-10-17 05:51:47.000000 dbcls-1.0.6/dbcls/sql_tokenizer.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-01-09 13:05:19.949006 dbcls-1.0.6/dbcls.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     1637 2024-01-09 13:05:19.000000 dbcls-1.0.6/dbcls.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      465 2024-01-09 13:05:19.000000 dbcls-1.0.6/dbcls.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-01-09 13:05:19.000000 dbcls-1.0.6/dbcls.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       37 2024-01-09 13:05:19.000000 dbcls-1.0.6/dbcls.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-08-31 06:22:39.000000 dbcls-1.0.6/dbcls.egg-info/not-zip-safe
--rw-r--r--   0 user       (501) staff       (20)      123 2024-01-09 13:05:19.000000 dbcls-1.0.6/dbcls.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        6 2024-01-09 13:05:19.000000 dbcls-1.0.6/dbcls.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)      123 2023-08-26 18:08:52.000000 dbcls-1.0.6/requirements.txt
--rw-r--r--   0 user       (501) staff       (20)       38 2024-01-09 13:05:19.949644 dbcls-1.0.6/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)     1005 2024-01-09 13:02:31.000000 dbcls-1.0.6/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-22 07:41:58.856373 dbcls-1.0.7/
+-rw-r--r--   0 user       (501) staff       (20)     1492 2023-08-26 08:16:50.000000 dbcls-1.0.7/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)       25 2023-08-26 18:36:21.000000 dbcls-1.0.7/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     1636 2024-05-22 07:41:58.856103 dbcls-1.0.7/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     1123 2023-08-26 19:12:56.000000 dbcls-1.0.7/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-22 07:41:58.851658 dbcls-1.0.7/dbcls/
+-rw-r--r--   0 user       (501) staff       (20)       24 2023-08-26 18:47:19.000000 dbcls-1.0.7/dbcls/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-22 07:41:58.854910 dbcls-1.0.7/dbcls/clients/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-08-26 13:23:14.000000 dbcls-1.0.7/dbcls/clients/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1405 2024-05-22 05:43:27.000000 dbcls-1.0.7/dbcls/clients/base.py
+-rw-r--r--   0 user       (501) staff       (20)     1361 2024-01-09 12:58:02.000000 dbcls-1.0.7/dbcls/clients/clickhouse.py
+-rw-r--r--   0 user       (501) staff       (20)     1143 2024-05-22 05:32:49.000000 dbcls-1.0.7/dbcls/clients/mysql.py
+-rw-r--r--   0 user       (501) staff       (20)     2226 2024-05-22 07:13:47.000000 dbcls-1.0.7/dbcls/clients/postgres.py
+-rw-r--r--   0 user       (501) staff       (20)     1407 2023-12-20 10:29:15.000000 dbcls-1.0.7/dbcls/clients/sqlite3.py
+-rw-r--r--   0 user       (501) staff       (20)    11661 2024-05-22 07:13:30.000000 dbcls-1.0.7/dbcls/dbcls.py
+-rw-r--r--   0 user       (501) staff       (20)     1826 2023-10-17 05:51:47.000000 dbcls-1.0.7/dbcls/sql_tokenizer.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-22 07:41:58.855795 dbcls-1.0.7/dbcls.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     1636 2024-05-22 07:41:58.000000 dbcls-1.0.7/dbcls.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      465 2024-05-22 07:41:58.000000 dbcls-1.0.7/dbcls.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-05-22 07:41:58.000000 dbcls-1.0.7/dbcls.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       37 2024-05-22 07:41:58.000000 dbcls-1.0.7/dbcls.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-08-31 06:22:39.000000 dbcls-1.0.7/dbcls.egg-info/not-zip-safe
+-rw-r--r--   0 user       (501) staff       (20)      122 2024-05-22 07:41:58.000000 dbcls-1.0.7/dbcls.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        6 2024-05-22 07:41:58.000000 dbcls-1.0.7/dbcls.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)      122 2024-05-22 07:14:30.000000 dbcls-1.0.7/requirements.txt
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-05-22 07:41:58.856422 dbcls-1.0.7/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)     1005 2024-05-22 07:40:22.000000 dbcls-1.0.7/setup.py
```

### Comparing `dbcls-1.0.6/LICENSE` & `dbcls-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dbcls-1.0.6/PKG-INFO` & `dbcls-1.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dbcls
-Version: 1.0.6
+Version: 1.0.7
 Summary: dbcls is a versatile client that supports various databases
 Author: Maksim Nikitenko
 Author-email: iam@sets88.com
 License: BSD
 Platform: any
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: kaaedit==0.54.0
-Requires-Dist: visidata==2.11.1
+Requires-Dist: visidata==3.0.2
 Requires-Dist: aiochclient[aiohttp]==2.4.0
 Requires-Dist: ciso8601==2.3.0
 Requires-Dist: aiomysql==0.2.0
 Requires-Dist: aiopg==1.4.0
 Requires-Dist: ssh_crypt==1.1.8
 
 # DbCls
```

### Comparing `dbcls-1.0.6/README.md` & `dbcls-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dbcls-1.0.6/dbcls/clients/base.py` & `dbcls-1.0.7/dbcls/clients/base.py`

 * *Files identical despite different names*

### Comparing `dbcls-1.0.6/dbcls/clients/clickhouse.py` & `dbcls-1.0.7/dbcls/clients/clickhouse.py`

 * *Files identical despite different names*

### Comparing `dbcls-1.0.6/dbcls/clients/mysql.py` & `dbcls-1.0.7/dbcls/clients/mysql.py`

 * *Files identical despite different names*

### Comparing `dbcls-1.0.6/dbcls/clients/postgres.py` & `dbcls-1.0.7/dbcls/clients/postgres.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,19 +30,24 @@
     async def execute(self, sql) -> Result:
         sql_stripped = sql.strip()
         first_word = sql_stripped.split(' ')[1]
 
         if sql_stripped.startswith('\\c '):
             db = first_word.rstrip(';')
             return await self.change_database(db)
+
         if sql_stripped.startswith('\\d '):
             sql = (
-                "SELECT column_name, data_type"
-                "FROM information_schema.columns"
+                "SELECT column_name, data_type "
+                "FROM information_schema.columns "
                 f"WHERE table_name = '{first_word}'"
+                "UNION ALL SELECT 'INDEXES', NULL "
+                "UNION ALL "
+                "SELECT indexname, indexdef "
+                f"FROM pg_indexes WHERE tablename = '{first_word}';"
             )
         if sql_stripped == ('\\d'):
             return await self.get_tables()
         if sql_stripped.startswith('\\l'):
             return await self.get_databases()
 
         async with aiopg.connect(
```

### Comparing `dbcls-1.0.6/dbcls/clients/sqlite3.py` & `dbcls-1.0.7/dbcls/clients/sqlite3.py`

 * *Files identical despite different names*

### Comparing `dbcls-1.0.6/dbcls/dbcls.py` & `dbcls-1.0.7/dbcls/dbcls.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,18 +216,19 @@
             end = time()
             message = 'Cancelled'
             return
 
         end = time()
         message = str(result)
 
-        if not result:
+        if not result or not result.data:
             return
 
         fix_visidata_curses()
+
         visidata.vd.run()
         visidata.vd.view(result.data)
     except Exception as exc:
         end = time()
         message = str(exc)
     finally:
         wnd.document.set_title(client.get_title())
```

### Comparing `dbcls-1.0.6/dbcls/sql_tokenizer.py` & `dbcls-1.0.7/dbcls/sql_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dbcls-1.0.6/dbcls.egg-info/PKG-INFO` & `dbcls-1.0.7/dbcls.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dbcls
-Version: 1.0.6
+Version: 1.0.7
 Summary: dbcls is a versatile client that supports various databases
 Author: Maksim Nikitenko
 Author-email: iam@sets88.com
 License: BSD
 Platform: any
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: kaaedit==0.54.0
-Requires-Dist: visidata==2.11.1
+Requires-Dist: visidata==3.0.2
 Requires-Dist: aiochclient[aiohttp]==2.4.0
 Requires-Dist: ciso8601==2.3.0
 Requires-Dist: aiomysql==0.2.0
 Requires-Dist: aiopg==1.4.0
 Requires-Dist: ssh_crypt==1.1.8
 
 # DbCls
```

### Comparing `dbcls-1.0.6/setup.py` & `dbcls-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         print(os.listdir(basedir))
         print(os.path.join(basedir, 'requirements.txt'))
         raise RuntimeError('No requirements info found.')
 
 
 setup(
     name='dbcls',
-    version='1.0.6',
+    version='1.0.7',
     license='BSD',
     author='Maksim Nikitenko',
     author_email='iam@sets88.com',
     packages=find_packages(),
     description='dbcls is a versatile client that supports various databases',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

