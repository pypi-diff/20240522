# Comparing `tmp/requirements_checker-0.1.8.tar.gz` & `tmp/requirements_checker-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requirements_checker-0.1.8.tar", last modified: Tue Feb  6 09:18:14 2024, max compression
+gzip compressed data, was "requirements_checker-0.1.9.tar", last modified: Thu Feb  8 13:27:22 2024, max compression
```

## Comparing `requirements_checker-0.1.8.tar` & `requirements_checker-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-02-06 09:18:14.798213 requirements_checker-0.1.8/
--rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 requirements_checker-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     2411 2024-02-06 09:18:14.798213 requirements_checker-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1462 2024-02-06 09:16:55.000000 requirements_checker-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-02-06 09:18:14.793214 requirements_checker-0.1.8/requirements_checker/
--rw-rw-rw-   0        0        0       85 2024-01-15 07:50:10.000000 requirements_checker-0.1.8/requirements_checker/__init__.py
--rw-rw-rw-   0        0        0    12550 2024-02-06 09:16:55.000000 requirements_checker-0.1.8/requirements_checker/check_pkg.py
--rw-rw-rw-   0        0        0    10669 2024-01-15 07:50:10.000000 requirements_checker-0.1.8/requirements_checker/check_string.py
--rw-rw-rw-   0        0        0       68 2023-12-18 08:01:14.000000 requirements_checker-0.1.8/requirements_checker/check_version.py
-drwxrwxrwx   0        0        0        0 2024-02-06 09:18:14.797213 requirements_checker-0.1.8/requirements_checker.egg-info/
--rw-rw-rw-   0        0        0     2411 2024-02-06 09:18:14.000000 requirements_checker-0.1.8/requirements_checker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-02-06 09:18:14.000000 requirements_checker-0.1.8/requirements_checker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-06 09:18:14.000000 requirements_checker-0.1.8/requirements_checker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-02-06 09:18:14.000000 requirements_checker-0.1.8/requirements_checker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-06 09:18:14.799214 requirements_checker-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 requirements_checker-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-08 13:27:22.603103 requirements_checker-0.1.9/
+-rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 requirements_checker-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     2411 2024-02-08 13:27:22.602968 requirements_checker-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1462 2024-02-08 13:26:35.000000 requirements_checker-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-02-08 13:27:22.592424 requirements_checker-0.1.9/requirements_checker/
+-rw-rw-rw-   0        0        0       85 2024-01-15 07:50:10.000000 requirements_checker-0.1.9/requirements_checker/__init__.py
+-rw-rw-rw-   0        0        0    12548 2024-02-08 12:23:27.000000 requirements_checker-0.1.9/requirements_checker/check_pkg.py
+-rw-rw-rw-   0        0        0    10669 2024-01-15 07:50:10.000000 requirements_checker-0.1.9/requirements_checker/check_string.py
+-rw-rw-rw-   0        0        0       68 2023-12-18 08:01:14.000000 requirements_checker-0.1.9/requirements_checker/check_version.py
+drwxrwxrwx   0        0        0        0 2024-02-08 13:27:22.601575 requirements_checker-0.1.9/requirements_checker.egg-info/
+-rw-rw-rw-   0        0        0     2411 2024-02-08 13:27:22.000000 requirements_checker-0.1.9/requirements_checker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-02-08 13:27:22.000000 requirements_checker-0.1.9/requirements_checker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-08 13:27:22.000000 requirements_checker-0.1.9/requirements_checker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-02-08 13:27:22.000000 requirements_checker-0.1.9/requirements_checker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-02-08 13:27:22.605275 requirements_checker-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 requirements_checker-0.1.9/setup.py
```

### Comparing `requirements_checker-0.1.8/LICENSE` & `requirements_checker-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `requirements_checker-0.1.8/PKG-INFO` & `requirements_checker-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirements_checker
-Version: 0.1.8
+Version: 0.1.9
 Summary: check if requirements met
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/requirements_checker
 Keywords: check requirements,check system requirements,raise/bool if no requirements,python packages work (upgrade/delete/version get)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# requirements_checker (v0.1.8)
+# requirements_checker (v0.1.9)
 
 ## DESCRIPTION_SHORT
 check if requirements met
 
 ## DESCRIPTION_LONG
 designed for check requirements (systemOs) and raise/bool if no match
```

### Comparing `requirements_checker-0.1.8/README.md` & `requirements_checker-0.1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# requirements_checker (v0.1.8)
+# requirements_checker (v0.1.9)
 
 ## DESCRIPTION_SHORT
 check if requirements met
 
 ## DESCRIPTION_LONG
 designed for check requirements (systemOs) and raise/bool if no match
```

### Comparing `requirements_checker-0.1.8/requirements_checker/check_pkg.py` & `requirements_checker-0.1.9/requirements_checker/check_pkg.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 
     def upgrade__centroid457(self) -> bool:
         return self.upgrade(self.PKGSET__CENTROID_457)
 
     # =================================================================================================================
     def upgrade_file(self, filepath: Union[str, pathlib.Path]) -> bool:
         filepath = pathlib.Path(filepath)
-        cmd = f"{self.PYTHON_PIP} install --upgrade -r '{filepath}'"
+        cmd = f"{self.PYTHON_PIP} install --upgrade -r {filepath}"
         return self.cli.send(cmd, timeout=60 * 5)
 
     def check_file(self, file) -> bool:
         # TODO: FINISH
         # TODO: FINISH
         # TODO: FINISH
         # TODO: FINISH
```

### Comparing `requirements_checker-0.1.8/requirements_checker/check_string.py` & `requirements_checker-0.1.9/requirements_checker/check_string.py`

 * *Files identical despite different names*

### Comparing `requirements_checker-0.1.8/requirements_checker.egg-info/PKG-INFO` & `requirements_checker-0.1.9/requirements_checker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirements_checker
-Version: 0.1.8
+Version: 0.1.9
 Summary: check if requirements met
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/requirements_checker
 Keywords: check requirements,check system requirements,raise/bool if no requirements,python packages work (upgrade/delete/version get)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# requirements_checker (v0.1.8)
+# requirements_checker (v0.1.9)
 
 ## DESCRIPTION_SHORT
 check if requirements met
 
 ## DESCRIPTION_LONG
 designed for check requirements (systemOs) and raise/bool if no match
```

### Comparing `requirements_checker-0.1.8/setup.py` & `requirements_checker-0.1.9/setup.py`

 * *Files identical despite different names*

