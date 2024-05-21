# Comparing `tmp/wwpdb.utils.db-0.31.tar.gz` & `tmp/wwpdb_utils_db-0.31.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.db-0.31.tar", last modified: Sat Apr  6 20:51:15 2024, max compression
+gzip compressed data, was "wwpdb_utils_db-0.31.1.tar", last modified: Tue May 21 23:08:43 2024, max compression
```

## Comparing `wwpdb.utils.db-0.31.tar` & `wwpdb_utils_db-0.31.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:51:15.157198 wwpdb.utils.db-0.31/
--rw-r--r--   0 vsts      (1001) docker     (127)     1026 2024-04-06 20:51:15.157198 wwpdb.utils.db-0.31/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      212 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-06 20:51:15.157198 wwpdb.utils.db-0.31/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2165 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:51:15.141197 wwpdb.utils.db-0.31/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:51:15.145197 wwpdb.utils.db-0.31/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:51:15.153198 wwpdb.utils.db-0.31/wwpdb/utils/db/
--rw-r--r--   0 vsts      (1001) docker     (127)   237963 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/BirdSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (127)   166675 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/ChemCompSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4802 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/DBLoadUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)   260559 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/DaInternalSchemaDef.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)    22118 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/DbLoadingApi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7042 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/MessageSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8889 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/MyConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19146 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/MyDbAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30645 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/MyDbSqlGen.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17636 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/MyDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23832 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/MyQueryDirectives.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4815 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/MysqlSchemaImporter.py
--rw-r--r--   0 vsts      (1001) docker     (127)   606730 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/PdbDistroSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (127)  3724930 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/PdbxSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12178 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/PdbxSchemaMapReader.py
--rw-r--r--   0 vsts      (1001) docker     (127)   150992 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/PrdChemCompSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15722 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/SchemaDefBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26185 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/SchemaDefLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7057 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/SqlLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12147 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistory.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6744 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistoryExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8873 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistorySchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (127)    32566 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistoryUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1829 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/StatusLoadWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27651 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/WorkflowSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:51:15.153198 wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1026 2024-04-06 20:51:15.000000 wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1177 2024-04-06 20:51:15.000000 wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-06 20:51:15.000000 wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-06 20:50:54.000000 wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      139 2024-04-06 20:51:15.000000 wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-06 20:51:15.000000 wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 23:08:43.347337 wwpdb_utils_db-0.31.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1028 2024-05-21 23:08:43.347337 wwpdb_utils_db-0.31.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      212 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-21 23:08:43.347337 wwpdb_utils_db-0.31.1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2165 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 23:08:43.331336 wwpdb_utils_db-0.31.1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 23:08:43.335337 wwpdb_utils_db-0.31.1/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 23:08:43.343337 wwpdb_utils_db-0.31.1/wwpdb/utils/db/
+-rw-r--r--   0 vsts      (1001) docker     (127)   237963 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/BirdSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   166675 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/ChemCompSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4802 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/DBLoadUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   260559 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/DaInternalSchemaDef.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    22118 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/DbLoadingApi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7042 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/MessageSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8889 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/MyConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19146 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/MyDbAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30831 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/MyDbSqlGen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17636 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/MyDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23832 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/MyQueryDirectives.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4815 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/MysqlSchemaImporter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   606730 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/PdbDistroSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)  3724930 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/PdbxSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12178 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/PdbxSchemaMapReader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   150992 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/PrdChemCompSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15722 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/SchemaDefBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26305 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/SchemaDefLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7057 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/SqlLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12147 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/StatusHistory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6744 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/StatusHistoryExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8873 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/StatusHistorySchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    32566 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/StatusHistoryUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1829 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/StatusLoadWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27651 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/WorkflowSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      156 2024-05-21 23:07:38.000000 wwpdb_utils_db-0.31.1/wwpdb/utils/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 23:08:43.343337 wwpdb_utils_db-0.31.1/wwpdb.utils.db.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1028 2024-05-21 23:08:43.000000 wwpdb_utils_db-0.31.1/wwpdb.utils.db.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1177 2024-05-21 23:08:43.000000 wwpdb_utils_db-0.31.1/wwpdb.utils.db.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 23:08:43.000000 wwpdb_utils_db-0.31.1/wwpdb.utils.db.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 23:08:27.000000 wwpdb_utils_db-0.31.1/wwpdb.utils.db.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      139 2024-05-21 23:08:43.000000 wwpdb_utils_db-0.31.1/wwpdb.utils.db.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-21 23:08:43.000000 wwpdb_utils_db-0.31.1/wwpdb.utils.db.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.db-0.31/PKG-INFO` & `wwpdb_utils_db-0.31.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.db
-Version: 0.31
+Version: 0.31.1
 Summary: wwPDB Python DB Schema Utilities
 Home-page: https://github.com/rcsb/py-wwpdb_utils_db
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.db-0.31/setup.py` & `wwpdb_utils_db-0.31.1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/BirdSchemaDef.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/BirdSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/ChemCompSchemaDef.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/ChemCompSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/DBLoadUtil.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/DBLoadUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/DaInternalSchemaDef.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/DaInternalSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/DbLoadingApi.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/DbLoadingApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/MessageSchemaDef.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/MessageSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/MyConnectionBase.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/MyConnectionBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/MyDbAdapter.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/MyDbAdapter.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/MyDbSqlGen.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/MyDbSqlGen.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 
     """Builds SQL commands to create table schema from a schema definition derived from class SchemaDefBase.
 
     Note:
     """
 
     def __init__(self, verbose=False, log=sys.stderr):  # pylint: disable=unused-argument
-        pass
+        self.__lfh = log
+        self.__verbose = verbose
 
     def truncateTableSQL(self, databaseName, tableName):
         """Return the SQL string require to truncate (remove all rows) from the input table."""
         return "TRUNCATE TABLE %s.%s; " % (databaseName, tableName)
 
     def idUpdateTemplateSQL(self, databaseName, tableDefObj, updateAttributeIdList=None, conditionAttributeIdList=None):
         """Return the SQL string template for updating the input attributes into the named table subject
@@ -265,15 +266,17 @@
                 tS = "%-40s %-16s  %s" % (name, sqlType, notNull)
             elif (sqlType == "TEXT") or (sqlType == "MEDIUMTEXT") or (sqlType == "LONGTEXT"):
                 tS = "%-40s %-16s  %s" % (name, sqlType, notNull)
             elif (sqlType == "DECIMAL") or (sqlType == "NUMERIC"):
                 sW = "%-s(%d,%d)" % (sqlType, width, precision)
                 tS = "%-40s %-16s  %s" % (name, sW, notNull)
             else:
-                pass
+                if self.__verbose:
+                    self.__lfh.write("+MyDbAdminSqlGen.__createTable unknown sqlType %s\n" % sqlType)
+                continue
             #
             # if ii < len(attributeIdList) -1:
             #    oL.append(tS+",")
             # else:
             #    oL.append(tS)
             oL.append(tS + ",")
```

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/MyDbUtil.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/MyDbUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/MyQueryDirectives.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/MyQueryDirectives.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/MysqlSchemaImporter.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/MysqlSchemaImporter.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/PdbDistroSchemaDef.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/PdbDistroSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/PdbxSchemaDef.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/PdbxSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/PdbxSchemaMapReader.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/PdbxSchemaMapReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/PrdChemCompSchemaDef.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/PrdChemCompSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/SchemaDefBase.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/SchemaDefBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/SchemaDefLoader.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/SchemaDefLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,16 @@
         Returns True for success or False otherwise.
 
         """
         if inputPathList is not None:
             tableDataDict, containerNameList = self.__fetch(inputPathList)
         elif containerList is not None:
             tableDataDict, containerNameList = self.__process(containerList)
+        else:
+            tableDataDict = containerNameList = []
         #
         #
         if self.__verbose:
             if len(self.__overWrite) > 0:
                 for k, v in self.__overWrite.items():
                     self.__lfh.write("+SchemaDefLoader(load) %r maximum width %r\n" % (k, v))
         #
@@ -314,14 +316,16 @@
                 #
                 otherAttributeIdList = tObj.getMapOtherAttributeIdList()
 
                 if numMapCategories == 1:
                     rowList = self.__mapInstanceCategory(tObj, mapCategoryNameList[0], myContainer)
                 elif numMapCategories >= 1:
                     rowList = self.__mapInstanceCategoryList(tObj, mapCategoryNameList, myContainer)
+                else:
+                    rowList = []
 
                 for atId in otherAttributeIdList:
                     fName = tObj.getMapAttributeFunction(atId)
                     fArgs = tObj.getMapAttributeFunctionArgs(atId)
                     self.__evalMapFunction(dataContainer=myContainer, rowList=rowList, attributeId=atId, functionName=fName, functionArgs=fArgs)
 
                 tableDataDict[tableId].extend(rowList)
```

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/SqlLoader.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/SqlLoader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistory.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/StatusHistory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistoryExec.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/StatusHistoryExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistorySchemaDef.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/StatusHistorySchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistoryUtils.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/StatusHistoryUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/StatusLoadWrapper.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/StatusLoadWrapper.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb/utils/db/WorkflowSchemaDef.py` & `wwpdb_utils_db-0.31.1/wwpdb/utils/db/WorkflowSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/PKG-INFO` & `wwpdb_utils_db-0.31.1/wwpdb.utils.db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.db
-Version: 0.31
+Version: 0.31.1
 Summary: wwPDB Python DB Schema Utilities
 Home-page: https://github.com/rcsb/py-wwpdb_utils_db
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/SOURCES.txt` & `wwpdb_utils_db-0.31.1/wwpdb.utils.db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

