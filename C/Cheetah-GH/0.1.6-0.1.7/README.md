# Comparing `tmp/cheetah_gh-0.1.6.tar.gz` & `tmp/cheetah_gh-0.1.7.tar.gz`

## Comparing `cheetah_gh-0.1.6.tar` & `cheetah_gh-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/.gitattributes
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/src/Cheetah_GH/__init__.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/src/Cheetah_GH/gh_and_py_runner.py
--rw-r--r--   0        0        0     9328 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/src/Cheetah_GH/helpers.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/src/Cheetah_GH/unittest_runner.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/LICENSE.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 cheetah_gh-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.1.7/.gitattributes
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cheetah_gh-0.1.7/src/Cheetah_GH/__init__.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 cheetah_gh-0.1.7/src/Cheetah_GH/gh_and_py_runner.py
+-rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 cheetah_gh-0.1.7/src/Cheetah_GH/helpers.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.1.7/src/Cheetah_GH/unittest_runner.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 cheetah_gh-0.1.7/LICENSE.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 cheetah_gh-0.1.7/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cheetah_gh-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 cheetah_gh-0.1.7/PKG-INFO
```

### Comparing `cheetah_gh-0.1.6/src/Cheetah_GH/gh_and_py_runner.py` & `cheetah_gh-0.1.7/src/Cheetah_GH/gh_and_py_runner.py`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.6/src/Cheetah_GH/helpers.py` & `cheetah_gh-0.1.7/src/Cheetah_GH/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,39 +134,40 @@
 def all_docs_comps():
    return {os.path.splitext(os.path.basename(doc.FilePath))[0] : (doc, GH_doc_components(doc)) 
            for doc in Grasshopper.Instances.DocumentServer.GetEnumerator() 
           }
 
 
 
-def get_plugin_files(plugin = ''):
+def get_plugin_files(plugin_name = ''):
 
     gh_comp_server = Grasshopper.Kernel.GH_ComponentServer()
     #print(list(gh_comp_server.FindObjects(guid)))
 
     return OrderedDict((os.path.splitext(file_.FileName)[0], file_)
                         for file_ in gh_comp_server.ExternalFiles(True, True)
-                        if plugin.lower() in file_.FilePath.lower()
+                        if plugin_name.lower() in file_.FilePath.lower()
                        )
 
 
 def get_position(comp_number, row_width = 800, row_height = 175, pos = (200, 550)):
     h = comp_number * row_height
     x = pos[0] + (h % row_width)
     y = pos[1] + 220 * (h // row_width)
     return x, y
 
 def add_instance_of_userobject_to_canvas(
     name,
-    plugin_files,
-    plug,
+    plugin_files = None,
+    plugin_name = '',
     comp_number=1,
     pos = (200, 550),
     ):
     
+    plugin_files = plugin_files or get_plugin_files(plugin_name)
     
     file_obj = next((v
                      for k, v in plugin_files.items() 
                      if name.lower() in k.lower()
                     )
                     ,None)
                     
@@ -211,18 +212,26 @@
     comp.ComputeData()
 
     return {param.NickName : get_data_from(param) 
             for param in comp.Params.Output
            }
 
 
-def get_user_obj_comp_from_or_add_to_canvas(name):
+def get_user_obj_comp_from_or_add_to_canvas(
+    name,
+    plugin_files = None,
+    plugin_name = '',
+    ):
     
     if name not in GH_DOC_COMPONENTS:
-        comp = add_instance_of_userobject_to_canvas(name)
+        comp = add_instance_of_userobject_to_canvas(
+                            name,
+                            plugin_files,
+                            plugin_name
+                            )
         GH_DOC_COMPONENTS[name] = comp
 
     return GH_DOC_COMPONENTS[name]
 
 
 class FileAndStream(object):
     def __init__(self, file, stream, print_too = False):
```

### Comparing `cheetah_gh-0.1.6/src/Cheetah_GH/unittest_runner.py` & `cheetah_gh-0.1.7/src/Cheetah_GH/unittest_runner.py`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.6/.gitignore` & `cheetah_gh-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.6/pyproject.toml` & `cheetah_gh-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 
 
 
 [project]
 name = "Cheetah_GH"
-version = "0.1.6"
+version = "0.1.7"
 authors = [{name = "James Parrott", email = "james.parrott@proton.me"}]
 description = "Runs Grasshopper components and stops Rhino from Python components. Optionally runs Rhino3D and Grasshopper from the command line."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=2.7"
 keywords = ["Rhino", "Grasshopper", "control", "components", "runner", "tests"]
 license = {file = "LICENSE.md"}
 classifiers = [
```

