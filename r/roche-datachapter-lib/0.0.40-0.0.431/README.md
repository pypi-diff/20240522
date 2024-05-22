# Comparing `tmp/roche_datachapter_lib-0.0.40.tar.gz` & `tmp/roche_datachapter_lib-0.0.431.tar.gz`

## Comparing `roche_datachapter_lib-0.0.40.tar` & `roche_datachapter_lib-0.0.431.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/requirements_for_build.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/requirements_for_test.txt
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/setup_build_upload.py
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/__domain__.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/__init__.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/data_transformer.py
--rw-r--r--   0        0        0     7402 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/db_config.py
--rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/google_services.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/google_services_enums.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/job_manager.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/logger.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/query_manager.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/result_type.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/simple_test.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/test_db_config.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/test_google_services.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/test_job_manager.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/test_query_manager.py
--rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/queries/ej_godw.sql
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/queries/ej_rexis.sql
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/queries/ej_sap.sql
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/queries/ej_sql_server.sql
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/queries/stock_sap.sql
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/LICENSE
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/README.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/pyproject.toml
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/PKG-INFO
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/requirements_for_build.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/requirements_for_test.txt
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/setup_build_upload.py
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/__domain__.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/__init__.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/data_transformer.py
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/db_config.py
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/google_services.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/google_services_enums.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/job_manager.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/logger.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/query_manager.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/result_type.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/tests/simple_test.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/tests/test_db_config.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/tests/test_google_services.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/tests/test_job_manager.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/tests/test_query_manager.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/tests/test_redshift_connection.py
+-rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/tests/queries/ej_godw.sql
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/tests/queries/ej_rexis.sql
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/tests/queries/ej_sap.sql
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/tests/queries/ej_sql_server.sql
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/tests/queries/stock_sap.sql
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/LICENSE
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/README.md
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/pyproject.toml
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.431/PKG-INFO
```

### Comparing `roche_datachapter_lib-0.0.40/setup_build_upload.py` & `roche_datachapter_lib-0.0.431/setup_build_upload.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/__domain__.py` & `roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/__domain__.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/data_transformer.py` & `roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/data_transformer.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/db_config.py` & `roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/db_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
                  "SQLSERVER_LATAM_AR_DB", "SQLSERVER_LATAM_AR_DEV_DB",
                  "SQLSERVER_LATAM_AR_FARMADB_DB", "SQLSERVER_LATAM_AR_SAND_DB",
                  "SQLSERVER_LATAM_AR_STAGING_DB", "SQLSERVER_LATAM_UY_DB",
                  "SQLSERVER_LATAM_UY_STAGING_DB", "GODW_SERVER", "GODW_PORT",
                  "GODW_USER", "GODW_PASSWORD", "GODW_SERVICENAME", "GODW_ORACLE_INSTANT_CLIENT_PATH",
                  "SAPDWP06_SERVER", "SAPDWP06_PORT", "SAPDWP06_USER", "SAPDWP06_PASSWORD", "SAPDWP06_DB",
                  "REXIS_SALES_SERVER", "REXIS_SALES_DB", "REXIS_SERVICES_SERVER", "REXIS_SERVICES_DB",
-                 "NEXUS_HOST", "NEXUS_DB", "NEXUS_PORT", "NEXUS_USER", "NEXUS_PASSWORD"]
+                 "NEXUS_HOST", "NEXUS_DB", "NEXUS_PORT", "NEXUS_USER", "NEXUS_PASSWORD",
+                 "RDI_LATAM_AR_USER", "RDI_LATAM_AR_PASSWORD", "RDI_LATAM_AR_HOST", "RDI_LATAM_AR_PORT", "RDI_LATAM_AR_DB"]
 
 for env_var_name in ENV_VAR_NAMES:
     value = environ.get(env_var_name)
     if value is not None:
         globals()[env_var_name] = value
     else:
         raise EnvironmentError(
@@ -46,15 +47,16 @@
         'sqlserver_latam_ar_staging': f"{SQLSERVER_BASE}/{SQLSERVER_LATAM_AR_STAGING_DB}",  # pylint:disable=undefined-variable
         'sqlserver_latam_uy': f"{SQLSERVER_BASE}/{SQLSERVER_LATAM_UY_DB}",  # pylint:disable=undefined-variable
         'sqlserver_latam_uy_staging': f"{SQLSERVER_BASE}/{SQLSERVER_LATAM_UY_STAGING_DB}",  # pylint:disable=undefined-variable
         'godw': f"oracle+oracledb://{GODW_USER}:{GODW_PASSWORD}@{GODW_SERVER}:{GODW_PORT}/?service_name={GODW_SERVICENAME}",  # pylint:disable=undefined-variable
         'sapdwp06': f"hana+hdbcli://{SAPDWP06_USER}:{SAPDWP06_PASSWORD}@{SAPDWP06_SERVER}:{SAPDWP06_PORT}/{SAPDWP06_DB}?encrypt=true",  # pylint:disable=undefined-variable
         'rexis_sales': f"mssql+pymssql://@{REXIS_SALES_SERVER}/{REXIS_SALES_DB}",  # pylint:disable=undefined-variable
         'rexis_services': f"mssql+pymssql://@{REXIS_SERVICES_SERVER}/{REXIS_SERVICES_DB}",  # pylint:disable=undefined-variable
-        'nexus_prod': f"mysql+pymysql://{NEXUS_USER}:{NEXUS_PASSWORD}@{NEXUS_HOST}:{NEXUS_PORT}/{NEXUS_DB}"  # pylint:disable=undefined-variable
+        'nexus_prod': f"mysql+pymysql://{NEXUS_USER}:{NEXUS_PASSWORD}@{NEXUS_HOST}:{NEXUS_PORT}/{NEXUS_DB}",  # pylint:disable=undefined-variable
+        'redshift': f"redshift+psycopg2://{RDI_LATAM_AR_USER}:{RDI_LATAM_AR_PASSWORD}@{RDI_LATAM_AR_HOST}:{RDI_LATAM_AR_PORT}/{RDI_LATAM_AR_DB}?sslmode=disable"  # pylint:disable=undefined-variable
     }
 
     @classmethod
     def __get_bind__(cls, bind: str = ''):
         return cls.SQLALCHEMY_BINDS[cls.validate_bind(bind)]
 
     @classmethod
@@ -121,17 +123,17 @@
                         print(type(valor))
                         input(valor)
                         raise ValueError(
                             "sp_params only accept dict of int, float, bool or str")
                 sql_string += ', '.join(params)
             connection.execute(text(sql_string))
             connection.commit()
-            
+
     @classmethod
-    def truncate_table(cls, p_bind: str, schema: str, table:str):
+    def truncate_table(cls, p_bind: str, schema: str, table: str):
         """Truncate specific table from specific bind"""
         engine = create_engine(cls.__get_bind__(p_bind))
         with engine.connect() as connection:
             sql_string = f"TRUNCATE TABLE [{str(schema)}].[{str(table)}]"
             connection.execute(text(sql_string))
             connection.commit()
             return True
```

### Comparing `roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/google_services.py` & `roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/google_services.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/job_manager.py` & `roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/job_manager.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/logger.py` & `roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/logger.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/query_manager.py` & `roche_datachapter_lib-0.0.431/src/roche_datachapter_lib/query_manager.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/tests/test_google_services.py` & `roche_datachapter_lib-0.0.431/tests/test_google_services.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/tests/test_job_manager.py` & `roche_datachapter_lib-0.0.431/tests/test_job_manager.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/tests/queries/ej_godw.sql` & `roche_datachapter_lib-0.0.431/tests/queries/ej_godw.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/tests/queries/ej_sap.sql` & `roche_datachapter_lib-0.0.431/tests/queries/ej_sap.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/tests/queries/ej_sql_server.sql` & `roche_datachapter_lib-0.0.431/tests/queries/ej_sql_server.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/tests/queries/stock_sap.sql` & `roche_datachapter_lib-0.0.431/tests/queries/stock_sap.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/.gitignore` & `roche_datachapter_lib-0.0.431/.gitignore`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/LICENSE` & `roche_datachapter_lib-0.0.431/LICENSE`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/README.md` & `roche_datachapter_lib-0.0.431/README.md`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/pyproject.toml` & `roche_datachapter_lib-0.0.431/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "roche_datachapter_lib"
-version = "0.0.40"
+version = "0.0.431"
 authors = [{ name = "Lucas Frías", email = "lucasmatiasfrias@live.com" }]
 description = "Esta biblioteca de código esta pensada para compartir funcionalidades entre todos los procesos ETL que desarrollemos con Python"
 readme = "README.md"
 requires-python = ">=3.12"
 dependencies = [
-    "Flask==2.3.1",
-    "Flask-SQLAlchemy==3.0.3",
+    "setuptools",
+    "pkginfo",
     "pymysql==1.1.0",
     "pymssql",
-    "oracledb==2.0.0",
+    "oracledb==2.2.0",
     "pyodbc==5.0.1",
+    "psycopg2-binary==2.9.9",
+    "sqlalchemy-redshift==0.8.14",
     "sqlalchemy-hana==1.1.1",
+    "Flask==3.0.3",
+    "Flask-SQLAlchemy==3.0.3",
     "pandas==2.1.3",
     "openpyxl==3.1.2",
     "google-api-python-client==2.99.0",
     "google-auth-httplib2==0.1.1",
     "google-auth-oauthlib==1.1.0",
     "chardet==5.2.0",
 ]
```

### Comparing `roche_datachapter_lib-0.0.40/PKG-INFO` & `roche_datachapter_lib-0.0.431/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.3
 Name: roche_datachapter_lib
-Version: 0.0.40
+Version: 0.0.431
 Summary: Esta biblioteca de código esta pensada para compartir funcionalidades entre todos los procesos ETL que desarrollemos con Python
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Lucas Frías <lucasmatiasfrias@live.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Requires-Dist: chardet==5.2.0
 Requires-Dist: flask-sqlalchemy==3.0.3
-Requires-Dist: flask==2.3.1
+Requires-Dist: flask==3.0.3
 Requires-Dist: google-api-python-client==2.99.0
 Requires-Dist: google-auth-httplib2==0.1.1
 Requires-Dist: google-auth-oauthlib==1.1.0
 Requires-Dist: openpyxl==3.1.2
-Requires-Dist: oracledb==2.0.0
+Requires-Dist: oracledb==2.2.0
 Requires-Dist: pandas==2.1.3
+Requires-Dist: pkginfo
+Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: pymssql
 Requires-Dist: pymysql==1.1.0
 Requires-Dist: pyodbc==5.0.1
+Requires-Dist: setuptools
 Requires-Dist: sqlalchemy-hana==1.1.1
+Requires-Dist: sqlalchemy-redshift==0.8.14
 Description-Content-Type: text/markdown
 
 # Roche Data Chapeter LIB
 
 ## Description
 It contains the base structure that includes the configuration parameters of the different databases using environment variables on the server, a static data_transformer class to perform the data transformation and another static class to perform connection to Google services through the Google REST API.
```

