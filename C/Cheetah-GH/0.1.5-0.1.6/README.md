# Comparing `tmp/cheetah_gh-0.1.5.tar.gz` & `tmp/cheetah_gh-0.1.6.tar.gz`

## Comparing `cheetah_gh-0.1.5.tar` & `cheetah_gh-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/.gitattributes
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/src/Cheetah_GH/__init__.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/src/Cheetah_GH/gh_and_py_runner.py
--rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/src/Cheetah_GH/helpers.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/src/Cheetah_GH/unittest_runner.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/LICENSE.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/.gitattributes
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/src/Cheetah_GH/__init__.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/src/Cheetah_GH/gh_and_py_runner.py
+-rw-r--r--   0        0        0     9328 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/src/Cheetah_GH/helpers.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/src/Cheetah_GH/unittest_runner.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/LICENSE.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/PKG-INFO
```

### Comparing `cheetah_gh-0.1.5/src/Cheetah_GH/gh_and_py_runner.py` & `cheetah_gh-0.1.6/src/Cheetah_GH/gh_and_py_runner.py`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.5/src/Cheetah_GH/helpers.py` & `cheetah_gh-0.1.6/src/Cheetah_GH/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 import rhinoscriptsyntax as rs
 
 
 TMP = tempfile.gettempdir()
 
 DIR = os.path.join(TMP, 'Cheetah_GH')
 
-os.makedirs(DIR)
+if not os.path.isdir(DIR):
+    os.makedirs(DIR) 
 
 try:
     ghdoc
 except NameError:
     import scriptcontext as sc
 
     if sc.doc == Rhino.RhinoDoc.ActiveDoc:
```

### Comparing `cheetah_gh-0.1.5/src/Cheetah_GH/unittest_runner.py` & `cheetah_gh-0.1.6/src/Cheetah_GH/unittest_runner.py`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.5/.gitignore` & `cheetah_gh-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.5/pyproject.toml` & `cheetah_gh-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 
 
 
 [project]
 name = "Cheetah_GH"
-version = "0.1.5"
+version = "0.1.6"
 authors = [{name = "James Parrott", email = "james.parrott@proton.me"}]
 description = "Runs Grasshopper components and stops Rhino from Python components. Optionally runs Rhino3D and Grasshopper from the command line."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=2.7"
 keywords = ["Rhino", "Grasshopper", "control", "components", "runner", "tests"]
 license = {file = "LICENSE.md"}
 classifiers = [
```

### Comparing `cheetah_gh-0.1.5/PKG-INFO` & `cheetah_gh-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: Cheetah_GH
-Version: 0.1.5
+Version: 0.1.6
 Summary: Runs Grasshopper components and stops Rhino from Python components. Optionally runs Rhino3D and Grasshopper from the command line.
 Project-URL: Homepage, https://github.com/JamesParrott/Cheetah_GH
 Project-URL: Bug Tracker, https://github.com/JamesParrott/Cheetah_GH/issues
 Author-email: James Parrott <james.parrott@proton.me>
 License-File: LICENSE.md
 Keywords: Grasshopper,Rhino,components,control,runner,tests
 Classifier: Programming Language :: Python
```

