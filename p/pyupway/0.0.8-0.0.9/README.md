# Comparing `tmp/pyupway-0.0.8.tar.gz` & `tmp/pyupway-0.0.9.tar.gz`

## Comparing `pyupway-0.0.8.tar` & `pyupway-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pyupway-0.0.8/changelog.md
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/config/__init__.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/config/myupwayconfig.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/enums/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/enums/dataservice.py
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/enums/variable.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/exceptions/__init__.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/exceptions/configurationerror.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/exceptions/loginerror.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/exceptions/responseerror.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/models/__init__.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/models/valuemodel.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/models/variablehistoryvalue.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/models/variablevalue.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/responses/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/responses/myupwayresponses.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/services/__init__.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/services/myuplinkservice.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pyupway-0.0.8/src/pyupway/services/myupwayservice.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 pyupway-0.0.8/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyupway-0.0.8/LICENSE
--rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 pyupway-0.0.8/README.md
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pyupway-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     8471 2020-02-02 00:00:00.000000 pyupway-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pyupway-0.0.9/changelog.md
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/config/__init__.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/config/myupwayconfig.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/enums/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/enums/dataservice.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/enums/variable.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/exceptions/__init__.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/exceptions/configurationerror.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/exceptions/loginerror.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/exceptions/responseerror.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/models/__init__.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/models/valuemodel.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/models/variablehistoryvalue.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/models/variablevalue.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/responses/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/responses/myupwayresponses.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/services/__init__.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/services/myuplinkservice.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pyupway-0.0.9/src/pyupway/services/myupwayservice.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 pyupway-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyupway-0.0.9/LICENSE
+-rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 pyupway-0.0.9/README.md
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pyupway-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     8471 2020-02-02 00:00:00.000000 pyupway-0.0.9/PKG-INFO
```

### Comparing `pyupway-0.0.8/src/pyupway/__init__.py` & `pyupway-0.0.9/src/pyupway/__init__.py`

 * *Files identical despite different names*

### Comparing `pyupway-0.0.8/src/pyupway/config/myupwayconfig.py` & `pyupway-0.0.9/src/pyupway/config/myupwayconfig.py`

 * *Files identical despite different names*

### Comparing `pyupway-0.0.8/src/pyupway/enums/variable.py` & `pyupway-0.0.9/src/pyupway/enums/variable.py`

 * *Files identical despite different names*

### Comparing `pyupway-0.0.8/src/pyupway/services/myuplinkservice.py` & `pyupway-0.0.9/src/pyupway/services/myuplinkservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,18 @@
         """
         No way to implement in new API.
         """
 
         results: List[VariableHistoryValue] = []
 
         return results
+    
+    def logout(self):
+        """ No implementation """
+        pass
 
     
     def _get_token(self):
         """
         Fetch new token from OAUTH
         """
```

### Comparing `pyupway-0.0.8/src/pyupway/services/myupwayservice.py` & `pyupway-0.0.9/src/pyupway/services/myupwayservice.py`

 * *Files identical despite different names*

### Comparing `pyupway-0.0.8/.gitignore` & `pyupway-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyupway-0.0.8/LICENSE` & `pyupway-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyupway-0.0.8/README.md` & `pyupway-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyupway-0.0.8/pyproject.toml` & `pyupway-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyupway"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Jussi Rosenberg", email="jussi.rosenberg@iki.fi" },
 ]
 description = "Read values from MyUpway cloud service"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pyupway-0.0.8/PKG-INFO` & `pyupway-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyupway
-Version: 0.0.8
+Version: 0.0.9
 Summary: Read values from MyUpway cloud service
 Project-URL: Homepage, https://github.com/lemanjo/pyupway
 Project-URL: Changelog, https://github.com/lemanjo/pyupway/blob/master/changelog.md
 Author-email: Jussi Rosenberg <jussi.rosenberg@iki.fi>
 License-File: LICENSE
 Keywords: Heat pump,Jäspi,MyUpway,Nibe
 Classifier: License :: OSI Approved :: MIT License
```

