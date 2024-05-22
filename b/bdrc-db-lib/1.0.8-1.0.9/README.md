# Comparing `tmp/bdrc_db_lib-1.0.8-py3-none-any.whl.zip` & `tmp/bdrc_db_lib-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 13927 bytes, number of entries: 16
+Zip file size: 13917 bytes, number of entries: 16
 -rw-r--r--  2.0 unx     3567 b- defN 23-Jan-23 22:51 BdrcDbLib/DBConfig.py
 -rw-r--r--  2.0 unx     7727 b- defN 23-Jan-23 22:51 BdrcDbLib/DbApp.py
 -rw-r--r--  2.0 unx     3510 b- defN 23-Jan-23 22:51 BdrcDbLib/DbAppParser.py
 -rw-r--r--  2.0 unx      122 b- defN 23-Jan-23 22:51 BdrcDbLib/SprocColumnError.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-23 19:45 BdrcDbLib/__init__.py
--rw-r--r--  2.0 unx     8487 b- defN 23-Jan-23 22:51 BdrcDbLib/DbOrm/DrsContextBase.py
+-rw-r--r--  2.0 unx     8484 b- defN 23-Jan-27 01:18 BdrcDbLib/DbOrm/DrsContextBase.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-23 19:16 BdrcDbLib/DbOrm/__init__.py
 -rw-r--r--  2.0 unx       16 b- defN 23-Jan-23 19:16 BdrcDbLib/DbOrm/models/__init__.py
 -rw-r--r--  2.0 unx     8505 b- defN 23-Jan-23 22:51 BdrcDbLib/DbOrm/models/drs.py
 -rw-r--r--  2.0 unx     2125 b- defN 23-Jan-23 22:51 Tests/DBConfigTest.py
 -rw-r--r--  2.0 unx       28 b- defN 23-Jan-23 22:51 Tests/__init__.py
 -rw-r--r--  2.0 unx     1189 b- defN 23-Jan-23 22:51 Tests/test_drs.py
--rw-r--r--  2.0 unx     1170 b- defN 23-Jan-25 00:55 bdrc_db_lib-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-25 00:55 bdrc_db_lib-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jan-25 00:55 bdrc_db_lib-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1278 b- defN 23-Jan-25 00:55 bdrc_db_lib-1.0.8.dist-info/RECORD
-16 files, 37832 bytes uncompressed, 11819 bytes compressed:  68.8%
+-rw-r--r--  2.0 unx     1143 b- defN 23-Jan-27 01:19 bdrc_db_lib-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jan-27 01:19 bdrc_db_lib-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jan-27 01:19 bdrc_db_lib-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1278 b- defN 23-Jan-27 01:19 bdrc_db_lib-1.0.9.dist-info/RECORD
+16 files, 37802 bytes uncompressed, 11809 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: Tests/__init__.py
 Comment: 
 
 Filename: Tests/test_drs.py
 Comment: 
 
-Filename: bdrc_db_lib-1.0.8.dist-info/METADATA
+Filename: bdrc_db_lib-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: bdrc_db_lib-1.0.8.dist-info/WHEEL
+Filename: bdrc_db_lib-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: bdrc_db_lib-1.0.8.dist-info/top_level.txt
+Filename: bdrc_db_lib-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: bdrc_db_lib-1.0.8.dist-info/RECORD
+Filename: bdrc_db_lib-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## BdrcDbLib/DbOrm/DrsContextBase.py

```diff
@@ -44,15 +44,15 @@
 
 class DrsDbContextBase:
     """
     Maintains and defines DRS Tables. Full ORM implementation
     """
 
     # Static class member so other apps can use it.
-    bdrc_db_conf: str = f"{'qa' if is_dev else 'prodcli'}:~/.config/bdrc/db_apps.config"
+    bdrc_db_conf: str = f"{'qa' if is_dev else 'prod'}:~/.config/bdrc/db_apps.config"
 
     @property
     def session(self) -> Session:
         return self.get_session()
 
     @staticmethod
     def get_session():
```

## Comparing `bdrc_db_lib-1.0.8.dist-info/METADATA` & `bdrc_db_lib-1.0.9.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdrc-db-lib
-Version: 1.0.8
+Version: 1.0.9
 Summary: BDRC Db Library
 Home-page: UNKNOWN
 Author: jimk
 Author-email: jimk@tbrc.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Requires-Dist: pymysql
 Requires-Dist: lxml
 Requires-Dist: sqlalchemy
 Requires-Dist: sqlalchemy-get-or-create
-Requires-Dist: mysqlclient
 
 bdrc-db-lib
 ===========
 
 Package which supports Uses an indirect config file for the database
 connection
```

## Comparing `bdrc_db_lib-1.0.8.dist-info/RECORD` & `bdrc_db_lib-1.0.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 BdrcDbLib/DBConfig.py,sha256=h8NwK6U0s7MKGUOFu_Ku4-HrQakT2TpiCarXP5JUfps,3567
 BdrcDbLib/DbApp.py,sha256=VC-bH5q7_OxamoZpT7OHGkGVi1ch908a3eI0rEqo2Ec,7727
 BdrcDbLib/DbAppParser.py,sha256=PRl9v2vcFP2wKtz5P_MpI7mWS1MuUkICxQ-OSE5_QXU,3510
 BdrcDbLib/SprocColumnError.py,sha256=8MGk7WSNtcR0dy1y_KAEkE3NAxs2ZI39Lg2M55ES0DM,122
 BdrcDbLib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-BdrcDbLib/DbOrm/DrsContextBase.py,sha256=CVZi0xRNUnjz9ChggP6mYdzkk-1UVFE5KYx4ocZkcVM,8487
+BdrcDbLib/DbOrm/DrsContextBase.py,sha256=-OMF_djoS6gFh1gSNw3MvxC41dK_A_OsV_WevG5810c,8484
 BdrcDbLib/DbOrm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 BdrcDbLib/DbOrm/models/__init__.py,sha256=ZqmtluWqc-EjCSEdyjzQB3MFtZKiO2gI-fFuDNgQ_4c,16
 BdrcDbLib/DbOrm/models/drs.py,sha256=aJlbjile0A2RxZvsPrWc1q_wRufYaRgA9MC1cDXfNDk,8505
 Tests/DBConfigTest.py,sha256=Bh4KDTBFeJW9YWxH6nCkmyVhg_JEoXLoHwq3z9gjkBQ,2125
 Tests/__init__.py,sha256=HDZk7gcYNBGhFSCHOgAzrMyp6eqWWHnkONiQ1V_pu_A,28
 Tests/test_drs.py,sha256=oF8VfPyR3_16mTr_gxC9Hm1KJGkRgDhUcYWHsBBgjHg,1189
-bdrc_db_lib-1.0.8.dist-info/METADATA,sha256=knlmn5hc_LTZFHC0LnoiqIuRYDpgOlSbB9ppL1pJgRM,1170
-bdrc_db_lib-1.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-bdrc_db_lib-1.0.8.dist-info/top_level.txt,sha256=Q4uxh4sRk0tB_l3GWrly8xVkmMk7tZHeH-CcPWQz2v8,16
-bdrc_db_lib-1.0.8.dist-info/RECORD,,
+bdrc_db_lib-1.0.9.dist-info/METADATA,sha256=tpg06jLE_1H4sFcHNNlLInyOOuwVHQrJEVNzY2sr-t4,1143
+bdrc_db_lib-1.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+bdrc_db_lib-1.0.9.dist-info/top_level.txt,sha256=Q4uxh4sRk0tB_l3GWrly8xVkmMk7tZHeH-CcPWQz2v8,16
+bdrc_db_lib-1.0.9.dist-info/RECORD,,
```

