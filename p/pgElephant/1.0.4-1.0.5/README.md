# Comparing `tmp/pgElephant-1.0.4.tar.gz` & `tmp/pgElephant-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgElephant-1.0.4.tar", last modified: Tue Mar 26 21:21:30 2024, max compression
+gzip compressed data, was "pgElephant-1.0.5.tar", last modified: Wed May 22 16:08:25 2024, max compression
```

## Comparing `pgElephant-1.0.4.tar` & `pgElephant-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 21:21:30.138520 pgElephant-1.0.4/
--rw-rw-rw-   0        0        0     1088 2024-03-24 20:58:31.000000 pgElephant-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     2099 2024-03-26 21:21:30.136519 pgElephant-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      555 2024-03-26 21:21:17.000000 pgElephant-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 21:21:30.106898 pgElephant-1.0.4/pgElephant/
--rw-rw-rw-   0        0        0       35 2024-03-24 21:22:30.000000 pgElephant-1.0.4/pgElephant/__init__.py
--rw-rw-rw-   0        0        0     2545 2024-03-26 21:17:12.000000 pgElephant-1.0.4/pgElephant/postgres.py
-drwxrwxrwx   0        0        0        0 2024-03-26 21:21:30.135013 pgElephant-1.0.4/pgElephant.egg-info/
--rw-rw-rw-   0        0        0     2099 2024-03-26 21:21:29.000000 pgElephant-1.0.4/pgElephant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-03-26 21:21:30.000000 pgElephant-1.0.4/pgElephant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 21:21:29.000000 pgElephant-1.0.4/pgElephant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-26 21:21:29.000000 pgElephant-1.0.4/pgElephant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-26 21:21:29.000000 pgElephant-1.0.4/pgElephant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-26 21:21:30.138520 pgElephant-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      569 2024-03-26 21:21:28.000000 pgElephant-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:08:25.104018 pgElephant-1.0.5/
+-rw-rw-rw-   0        0        0     1088 2024-05-22 15:59:26.000000 pgElephant-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2039 2024-05-22 16:08:25.103017 pgElephant-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2024-05-22 16:05:59.000000 pgElephant-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 16:08:25.077557 pgElephant-1.0.5/pgElephant/
+-rw-rw-rw-   0        0        0       35 2024-05-22 15:59:52.000000 pgElephant-1.0.5/pgElephant/__init__.py
+-rw-rw-rw-   0        0        0     2435 2024-05-22 16:02:45.000000 pgElephant-1.0.5/pgElephant/postgres.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:08:25.101016 pgElephant-1.0.5/pgElephant.egg-info/
+-rw-rw-rw-   0        0        0     2039 2024-05-22 16:08:25.000000 pgElephant-1.0.5/pgElephant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2024-05-22 16:08:25.000000 pgElephant-1.0.5/pgElephant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 16:08:25.000000 pgElephant-1.0.5/pgElephant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-22 16:08:25.000000 pgElephant-1.0.5/pgElephant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-22 16:08:25.000000 pgElephant-1.0.5/pgElephant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 16:08:25.104018 pgElephant-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      569 2024-05-22 16:02:58.000000 pgElephant-1.0.5/setup.py
```

### Comparing `pgElephant-1.0.4/LICENSE` & `pgElephant-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pgElephant-1.0.4/PKG-INFO` & `pgElephant-1.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgElephant
-Version: 1.0.4
+Version: 1.0.5
 Summary: PostgreSQL Database Manager
 Author: Ryan Souza Anselmo
 Author-email: ryansouza.cwb@gmail.com
 License: MIT License
         
         Copyright (c) 2024 Ryan Souza
         
@@ -25,33 +25,32 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Keywords: pgElephant
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: psycopg2
 
 # pgElephant
 PostgreSQL Database Manager
 
 # CREATE ADMIN
-bank = PostgreSQL(dbname='sgo',user='dev',password=123456)
+bank = PostgreSQL(dbname='my_db',user='my_user',password=my_password)
 
 # CONNECT
 bank.connect()
 
 # CHECK
 version = bank.version()
 
 # GET ALL VALUES IN ONE TABLE
 value_all = bank.get_all(table='users')
 
-# GET A UNIQUE ITEM
-value_single = bank.get_single(unique='ryansouza.cwb@gmail.com',table='users',column='email')
+# GET A ID
+value_single = bank.get_single(id='my_id',table='users')
 
 # GET A SINGLE LINE
 value_first = bank.get_first(unique='ryansouza.cwb@gmail.com',table='users',column='email')
 
 # COMMIT
 bank.commit()
```

### Comparing `pgElephant-1.0.4/README.md` & `pgElephant-1.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # pgElephant
 PostgreSQL Database Manager
 
 # CREATE ADMIN
-bank = PostgreSQL(dbname='sgo',user='dev',password=123456)
+bank = PostgreSQL(dbname='my_db',user='my_user',password=my_password)
 
 # CONNECT
 bank.connect()
 
 # CHECK
 version = bank.version()
 
 # GET ALL VALUES IN ONE TABLE
 value_all = bank.get_all(table='users')
 
-# GET A UNIQUE ITEM
-value_single = bank.get_single(unique='ryansouza.cwb@gmail.com',table='users',column='email')
+# GET A ID
+value_single = bank.get_single(id='my_id',table='users')
 
 # GET A SINGLE LINE
 value_first = bank.get_first(unique='ryansouza.cwb@gmail.com',table='users',column='email')
 
 # COMMIT
 bank.commit()
```

### Comparing `pgElephant-1.0.4/pgElephant/postgres.py` & `pgElephant-1.0.5/pgElephant/postgres.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,25 +46,21 @@
             result = {}
             for i in range(len(columns)):
                 result[columns[i]] = row[i]
             results.append(result)
 
         return results
     
-    def get_single(self, unique: str, table: str, column: str):
-        self.execute(f"SELECT * FROM {table} WHERE {column} LIKE %s", ('%' + unique + '%',))
+    def get_single(self, id: str, table: str):
+        self.execute(f"SELECT * FROM {table} WHERE id = %s", (id,))
         result = self._cursor.fetchone()
 
         if result is not None:
-            columns = [column[0] for column in self._cursor.description]
-            
-            result_dict = {}
-            for i in range(len(columns)):
-                result_dict[columns[i]] = result[i]
-
+            columns = [col[0] for col in self._cursor.description]
+            result_dict = {columns[i]: result[i] for i in range(len(columns))}
             return result_dict
         else:
             return None
 
     def get_first(self, unique: str, table: str, column: str):
         self.execute(f"SELECT * FROM {table} WHERE {column} LIKE %s", ('%' + unique + '%',))
         result = self._cursor.fetchone()
```

### Comparing `pgElephant-1.0.4/pgElephant.egg-info/PKG-INFO` & `pgElephant-1.0.5/pgElephant.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgElephant
-Version: 1.0.4
+Version: 1.0.5
 Summary: PostgreSQL Database Manager
 Author: Ryan Souza Anselmo
 Author-email: ryansouza.cwb@gmail.com
 License: MIT License
         
         Copyright (c) 2024 Ryan Souza
         
@@ -25,33 +25,32 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Keywords: pgElephant
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: psycopg2
 
 # pgElephant
 PostgreSQL Database Manager
 
 # CREATE ADMIN
-bank = PostgreSQL(dbname='sgo',user='dev',password=123456)
+bank = PostgreSQL(dbname='my_db',user='my_user',password=my_password)
 
 # CONNECT
 bank.connect()
 
 # CHECK
 version = bank.version()
 
 # GET ALL VALUES IN ONE TABLE
 value_all = bank.get_all(table='users')
 
-# GET A UNIQUE ITEM
-value_single = bank.get_single(unique='ryansouza.cwb@gmail.com',table='users',column='email')
+# GET A ID
+value_single = bank.get_single(id='my_id',table='users')
 
 # GET A SINGLE LINE
 value_first = bank.get_first(unique='ryansouza.cwb@gmail.com',table='users',column='email')
 
 # COMMIT
 bank.commit()
```

### Comparing `pgElephant-1.0.4/setup.py` & `pgElephant-1.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = arquivo.read()
 
 with open("LICENSE", "r") as arquivo:
     licence = arquivo.read()
 
 setup(name='pgElephant',
 
-    version='1.0.4',
+    version='1.0.5',
 
     license=licence,
 
     author='Ryan Souza Anselmo',
 
     long_description=readme,
```

