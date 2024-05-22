# Comparing `tmp/qase_robotframework-3.0.0b3.tar.gz` & `tmp/qase_robotframework-3.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase_robotframework-3.0.0b3.tar", last modified: Mon May 20 12:44:40 2024, max compression
+gzip compressed data, was "qase_robotframework-3.0.0b4.tar", last modified: Wed May 22 10:47:59 2024, max compression
```

## Comparing `qase_robotframework-3.0.0b3.tar` & `qase_robotframework-3.0.0b4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:44:40.076422 qase_robotframework-3.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-20 12:44:31.000000 qase_robotframework-3.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-05-20 12:44:40.076422 qase_robotframework-3.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-20 12:44:31.000000 qase_robotframework-3.0.0b3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-20 12:44:31.000000 qase_robotframework-3.0.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:44:40.076422 qase_robotframework-3.0.0b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:44:40.072422 qase_robotframework-3.0.0b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:44:40.072422 qase_robotframework-3.0.0b3/src/qase/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:44:40.072422 qase_robotframework-3.0.0b3/src/qase/robotframework/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 12:44:31.000000 qase_robotframework-3.0.0b3/src/qase/robotframework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-20 12:44:31.000000 qase_robotframework-3.0.0b3/src/qase/robotframework/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-20 12:44:31.000000 qase_robotframework-3.0.0b3/src/qase/robotframework/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 12:44:31.000000 qase_robotframework-3.0.0b3/src/qase/robotframework/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:44:40.072422 qase_robotframework-3.0.0b3/src/qase_robotframework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-05-20 12:44:40.000000 qase_robotframework-3.0.0b3/src/qase_robotframework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-20 12:44:40.000000 qase_robotframework-3.0.0b3/src/qase_robotframework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:44:40.000000 qase_robotframework-3.0.0b3/src/qase_robotframework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 12:44:40.000000 qase_robotframework-3.0.0b3/src/qase_robotframework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 12:44:40.000000 qase_robotframework-3.0.0b3/src/qase_robotframework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:47:59.849076 qase_robotframework-3.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-22 10:47:51.000000 qase_robotframework-3.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-05-22 10:47:59.849076 qase_robotframework-3.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-22 10:47:51.000000 qase_robotframework-3.0.0b4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-22 10:47:51.000000 qase_robotframework-3.0.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:47:59.849076 qase_robotframework-3.0.0b4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:47:59.845076 qase_robotframework-3.0.0b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:47:59.845076 qase_robotframework-3.0.0b4/src/qase/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:47:59.849076 qase_robotframework-3.0.0b4/src/qase/robotframework/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 10:47:51.000000 qase_robotframework-3.0.0b4/src/qase/robotframework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-22 10:47:51.000000 qase_robotframework-3.0.0b4/src/qase/robotframework/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-22 10:47:51.000000 qase_robotframework-3.0.0b4/src/qase/robotframework/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-22 10:47:51.000000 qase_robotframework-3.0.0b4/src/qase/robotframework/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:47:59.849076 qase_robotframework-3.0.0b4/src/qase_robotframework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-05-22 10:47:59.000000 qase_robotframework-3.0.0b4/src/qase_robotframework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-22 10:47:59.000000 qase_robotframework-3.0.0b4/src/qase_robotframework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:47:59.000000 qase_robotframework-3.0.0b4/src/qase_robotframework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 10:47:59.000000 qase_robotframework-3.0.0b4/src/qase_robotframework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 10:47:59.000000 qase_robotframework-3.0.0b4/src/qase_robotframework.egg-info/top_level.txt
```

### Comparing `qase_robotframework-3.0.0b3/LICENSE` & `qase_robotframework-3.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `qase_robotframework-3.0.0b3/PKG-INFO` & `qase_robotframework-3.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-robotframework
-Version: 3.0.0b3
+Version: 3.0.0b4
 Summary: Qase Robot Framework Plugin
 Author-email: Qase Team <support@qase.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qase_robotframework-3.0.0b3/README.md` & `qase_robotframework-3.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `qase_robotframework-3.0.0b3/pyproject.toml` & `qase_robotframework-3.0.0b4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-robotframework"
-version = "3.0.0b3"
+version = "3.0.0b4"
 description = "Qase Robot Framework Plugin"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Robot Framework",
```

### Comparing `qase_robotframework-3.0.0b3/src/qase/robotframework/listener.py` & `qase_robotframework-3.0.0b4/src/qase/robotframework/listener.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -44,22 +44,22 @@
         logger.debug("Starting suite '%s'", name)
 
     def start_test(self, name, attributes: StartTestModel):
         logger.debug("Starting test '%s'", name)
 
         self.runtime.result = Result(title=name, signature=name)
         self.runtime.steps = {}
-        case_id = self._extract_ids(attributes.get("tags"))
-
-        if case_id:
-            self.runtime.result.testops_id = int(case_id)
 
     def end_test(self, name, attributes: EndTestModel):
         logger.debug("Finishing test '%s'", name)
 
+        case_id = self._extract_ids(attributes.get("tags"))
+        if case_id:
+            self.runtime.result.testops_id = int(case_id)
+
         self.runtime.result.execution.complete()
         self.runtime.result.execution.set_status(STATUSES[attributes.get("status")])
         self.runtime.result.execution.stacktrace = attributes.get("message")
         self.runtime.result.add_steps([step for key, step in self.runtime.steps.items()])
 
         self.runtime.result.add_field(Field("description", attributes.get("doc")))
```

### Comparing `qase_robotframework-3.0.0b3/src/qase/robotframework/models.py` & `qase_robotframework-3.0.0b4/src/qase/robotframework/models.py`

 * *Files identical despite different names*

### Comparing `qase_robotframework-3.0.0b3/src/qase_robotframework.egg-info/PKG-INFO` & `qase_robotframework-3.0.0b4/src/qase_robotframework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-robotframework
-Version: 3.0.0b3
+Version: 3.0.0b4
 Summary: Qase Robot Framework Plugin
 Author-email: Qase Team <support@qase.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

