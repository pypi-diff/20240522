# Comparing `tmp/tfdocs-1.0.9.tar.gz` & `tmp/tfdocs-1.1.tar.gz`

## Comparing `tfdocs-1.0.9.tar` & `tfdocs-1.1.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 tfdocs-1.0.9/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 tfdocs-1.0.9/src/tfdocs/__init__.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 tfdocs-1.0.9/src/tfdocs/__main__.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 tfdocs-1.0.9/src/tfdocs/cli.py
--rw-r--r--   0        0        0     6971 2020-02-02 00:00:00.000000 tfdocs-1.0.9/src/tfdocs/readme.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 tfdocs-1.0.9/src/tfdocs/utils.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 tfdocs-1.0.9/src/tfdocs/version.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 tfdocs-1.0.9/LICENCE
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 tfdocs-1.0.9/README.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 tfdocs-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 tfdocs-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tfdocs-1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 tfdocs-1.1/src/tfdocs/__init__.py
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 tfdocs-1.1/src/tfdocs/__main__.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 tfdocs-1.1/src/tfdocs/cli.py
+-rw-r--r--   0        0        0     7014 2020-02-02 00:00:00.000000 tfdocs-1.1/src/tfdocs/readme.py
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 tfdocs-1.1/src/tfdocs/utils.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 tfdocs-1.1/src/tfdocs/version.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 tfdocs-1.1/tests/readme_test.py
+-rw-r--r--   0        0        0    13264 2020-02-02 00:00:00.000000 tfdocs-1.1/tests/utils_test.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 tfdocs-1.1/LICENCE
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 tfdocs-1.1/README.md
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 tfdocs-1.1/pyproject.toml
+-rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 tfdocs-1.1/PKG-INFO
```

### Comparing `tfdocs-1.0.9/src/tfdocs/__init__.py` & `tfdocs-1.1/src/tfdocs/__init__.py`

 * *Files identical despite different names*

### Comparing `tfdocs-1.0.9/src/tfdocs/__main__.py` & `tfdocs-1.1/src/tfdocs/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,15 +43,21 @@
         print(f"tfdocs {cli.get_version()}")
         sys.exit(0)
 
     module_name = (
         options.module_name if options.module_name else os.getcwd().split("/")[-1]
     )
 
-    rd = readme.Readme(options.readme_file, options.variables_file, module_name, options.source, options.git_source)
+    rd = readme.Readme(
+        options.readme_file,
+        options.variables_file,
+        module_name,
+        options.source,
+        options.git_source,
+    )
     if not options.dry_run and options.format:
         rd.write_variables()
 
     if options.dry_run:
         if options.format:
             rd.print_variables_file()
             if not rd.get_status()["variables"]:
```

### Comparing `tfdocs-1.0.9/src/tfdocs/cli.py` & `tfdocs-1.1/src/tfdocs/cli.py`

 * *Files identical despite different names*

### Comparing `tfdocs-1.0.9/src/tfdocs/readme.py` & `tfdocs-1.1/src/tfdocs/readme.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,20 @@
     generate_source,
     process_line_block,
 )
 
 
 class Readme:
     def __init__(
-        self, readme_file, variables_file, module_name=None, module_source=None, module_source_git=False
+        self,
+        readme_file,
+        variables_file,
+        module_name=None,
+        module_source=None,
+        module_source_git=False,
     ):
         self.module_name = module_name
         self.module_source = module_source
         self.module_source_git = module_source_git
         self.readme_content: str
         self.readme_changed = True
         self.variables_changed = True
@@ -81,15 +86,15 @@
                     block = []
                     attributes = {
                         "name": name,
                         "type_override": type_override,
                         "type": type_content if type_content else "unknown",
                         "description": description_content
                         if description_content
-                        else "No description provided",
+                        else '"No description provided"',
                     }
 
                     if default_content:
                         attributes["default"] = default_content
 
                     self.variables.append(attributes)
```

### Comparing `tfdocs-1.0.9/src/tfdocs/utils.py` & `tfdocs-1.1/src/tfdocs/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,19 +54,20 @@
 
     return content, cont
 
 
 def match_type_constructors(string):
     type_constructors = ["list", "set", "map", "object", "tuple"]
 
-    for sub in type_constructors:
-        if sub in string:
-            return True
+    pattern = r"\b(" + "|".join(type_constructors) + r")\b"
 
-    return False
+    if re.search(pattern, string):
+        return True
+    else:
+        return False
 
 
 def format_block(content):
     start_braces = ["{", "[", "("]
     end_braces = ["}", "]", ")"]
     prev_item = None
     tmp_content = ""
```

### Comparing `tfdocs-1.0.9/LICENCE` & `tfdocs-1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `tfdocs-1.0.9/README.md` & `tfdocs-1.1/README.md`

 * *Files identical despite different names*

### Comparing `tfdocs-1.0.9/pyproject.toml` & `tfdocs-1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 
 [tool.hatch.version]
 path = "src/tfdocs/version.py"
 
 [project.scripts]
 tfdocs = "tfdocs.__main__:main"
 
+[tool.pytest.ini_options]
+pythonpath = [
+  ".", "src",
+]
+
 [project]
 name = "tfdocs"
 
 dependencies = [
     "rich>=12.0.0",
     "GitPython>=3.1.30"
 ]
```

### Comparing `tfdocs-1.0.9/PKG-INFO` & `tfdocs-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tfdocs
-Version: 1.0.9
+Version: 1.1
 Summary: Documentation generator for Terraform modules
 Project-URL: Homepage, https://github.com/vajeen/tfdocs
 Project-URL: Issues, https://github.com/vajeen/tfdocs/issues
 Author-email: Vajeen Karunathilaka <vajeen@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

