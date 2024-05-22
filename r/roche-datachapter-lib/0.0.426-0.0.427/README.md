# Comparing `tmp/roche_datachapter_lib-0.0.426.tar.gz` & `tmp/roche_datachapter_lib-0.0.427.tar.gz`

## Comparing `roche_datachapter_lib-0.0.426.tar` & `roche_datachapter_lib-0.0.427.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/requirements_for_build.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/requirements_for_test.txt
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/setup_build_upload.py
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/__domain__.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/__init__.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/data_transformer.py
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/db_config.py
--rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/google_services.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/google_services_enums.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/job_manager.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/logger.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/query_manager.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/result_type.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/tests/simple_test.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/tests/test_db_config.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/tests/test_google_services.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/tests/test_job_manager.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/tests/test_query_manager.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/tests/test_redshift_connection.py
--rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/tests/queries/ej_godw.sql
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/tests/queries/ej_rexis.sql
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/tests/queries/ej_sap.sql
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/tests/queries/ej_sql_server.sql
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/tests/queries/stock_sap.sql
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/LICENSE
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/README.md
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/pyproject.toml
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.426/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/requirements_for_build.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/requirements_for_test.txt
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/setup_build_upload.py
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/__domain__.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/__init__.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/data_transformer.py
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/db_config.py
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/google_services.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/google_services_enums.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/job_manager.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/logger.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/query_manager.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/result_type.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/tests/simple_test.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/tests/test_db_config.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/tests/test_google_services.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/tests/test_job_manager.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/tests/test_query_manager.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/tests/test_redshift_connection.py
+-rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/tests/queries/ej_godw.sql
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/tests/queries/ej_rexis.sql
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/tests/queries/ej_sap.sql
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/tests/queries/ej_sql_server.sql
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/tests/queries/stock_sap.sql
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/LICENSE
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/README.md
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/pyproject.toml
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.427/PKG-INFO
```

### Comparing `roche_datachapter_lib-0.0.426/setup_build_upload.py` & `roche_datachapter_lib-0.0.427/setup_build_upload.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/__domain__.py` & `roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/__domain__.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/data_transformer.py` & `roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/data_transformer.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/db_config.py` & `roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/db_config.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/google_services.py` & `roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/google_services.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/job_manager.py` & `roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/job_manager.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/logger.py` & `roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/logger.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/src/roche_datachapter_lib/query_manager.py` & `roche_datachapter_lib-0.0.427/src/roche_datachapter_lib/query_manager.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/tests/test_google_services.py` & `roche_datachapter_lib-0.0.427/tests/test_google_services.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/tests/test_job_manager.py` & `roche_datachapter_lib-0.0.427/tests/test_job_manager.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/tests/test_redshift_connection.py` & `roche_datachapter_lib-0.0.427/tests/test_redshift_connection.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/tests/queries/ej_godw.sql` & `roche_datachapter_lib-0.0.427/tests/queries/ej_godw.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/tests/queries/ej_sap.sql` & `roche_datachapter_lib-0.0.427/tests/queries/ej_sap.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/tests/queries/ej_sql_server.sql` & `roche_datachapter_lib-0.0.427/tests/queries/ej_sql_server.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/tests/queries/stock_sap.sql` & `roche_datachapter_lib-0.0.427/tests/queries/stock_sap.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/.gitignore` & `roche_datachapter_lib-0.0.427/.gitignore`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/LICENSE` & `roche_datachapter_lib-0.0.427/LICENSE`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/README.md` & `roche_datachapter_lib-0.0.427/README.md`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.426/PKG-INFO` & `roche_datachapter_lib-0.0.427/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.3
 Name: roche_datachapter_lib
-Version: 0.0.426
+Version: 0.0.427
 Summary: Esta biblioteca de código esta pensada para compartir funcionalidades entre todos los procesos ETL que desarrollemos con Python
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Lucas Frías <lucasmatiasfrias@live.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
-Requires-Dist: chardet==5.2.0
-Requires-Dist: flask-sqlalchemy==3.0.3
-Requires-Dist: flask==3.0.3
-Requires-Dist: google-api-python-client==2.99.0
-Requires-Dist: google-auth-httplib2==0.1.1
-Requires-Dist: google-auth-oauthlib==1.1.0
-Requires-Dist: openpyxl==3.1.2
-Requires-Dist: oracledb==2.2.0
-Requires-Dist: pandas==2.1.3
+Requires-Dist: chardet
+Requires-Dist: flask
+Requires-Dist: flask-sqlalchemy
+Requires-Dist: google-api-python-client
+Requires-Dist: google-auth-httplib2
+Requires-Dist: google-auth-oauthlib
+Requires-Dist: openpyxl
+Requires-Dist: oracledb
+Requires-Dist: pandas
 Requires-Dist: pkginfo
-Requires-Dist: psycopg2-binary==2.9.9
+Requires-Dist: psycopg2-binary
 Requires-Dist: pymssql
-Requires-Dist: pymysql==1.1.0
-Requires-Dist: pyodbc==5.0.1
-Requires-Dist: sqlalchemy-hana==1.1.1
-Requires-Dist: sqlalchemy-redshift==0.8.14
+Requires-Dist: pymysql
+Requires-Dist: pyodbc
+Requires-Dist: sqlalchemy-hana
+Requires-Dist: sqlalchemy-redshift
 Description-Content-Type: text/markdown
 
 # Roche Data Chapeter LIB
 
 ## Description
 It contains the base structure that includes the configuration parameters of the different databases using environment variables on the server, a static data_transformer class to perform the data transformation and another static class to perform connection to Google services through the Google REST API.
```

