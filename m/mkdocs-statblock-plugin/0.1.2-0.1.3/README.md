# Comparing `tmp/mkdocs_statblock_plugin-0.1.2.tar.gz` & `tmp/mkdocs_statblock_plugin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_statblock_plugin-0.1.2.tar", last modified: Mon May 20 13:25:19 2024, max compression
+gzip compressed data, was "mkdocs_statblock_plugin-0.1.3.tar", last modified: Tue May 21 21:34:58 2024, max compression
```

## Comparing `mkdocs_statblock_plugin-0.1.2.tar` & `mkdocs_statblock_plugin-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-20 13:25:19.792955 mkdocs_statblock_plugin-0.1.2/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1054 2024-05-20 12:27:56.000000 mkdocs_statblock_plugin-0.1.2/LICENSE
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2173 2024-05-20 13:25:19.792955 mkdocs_statblock_plugin-0.1.2/PKG-INFO
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1753 2024-05-20 12:14:05.000000 mkdocs_statblock_plugin-0.1.2/README.md
-drwxr-xr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-20 13:25:19.792955 mkdocs_statblock_plugin-0.1.2/mkdocs_statblock_plugin/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2024-05-20 09:39:13.000000 mkdocs_statblock_plugin-0.1.2/mkdocs_statblock_plugin/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1368 2024-05-20 12:42:28.000000 mkdocs_statblock_plugin-0.1.2/mkdocs_statblock_plugin/mkdocs_statblock_plugin.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2273 2024-05-20 12:42:30.000000 mkdocs_statblock_plugin-0.1.2/mkdocs_statblock_plugin/statblock_handler.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     3372 2024-05-20 11:50:52.000000 mkdocs_statblock_plugin-0.1.2/mkdocs_statblock_plugin/template.html
-drwxr-xr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-20 13:25:19.792955 mkdocs_statblock_plugin-0.1.2/mkdocs_statblock_plugin.egg-info/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2173 2024-05-20 13:25:19.000000 mkdocs_statblock_plugin-0.1.2/mkdocs_statblock_plugin.egg-info/PKG-INFO
--rw-r--r--   0 johannes  (1000) johannes  (1000)      480 2024-05-20 13:25:19.000000 mkdocs_statblock_plugin-0.1.2/mkdocs_statblock_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)        1 2024-05-20 13:25:19.000000 mkdocs_statblock_plugin-0.1.2/mkdocs_statblock_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)       94 2024-05-20 13:25:19.000000 mkdocs_statblock_plugin-0.1.2/mkdocs_statblock_plugin.egg-info/entry_points.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)       21 2024-05-20 13:25:19.000000 mkdocs_statblock_plugin-0.1.2/mkdocs_statblock_plugin.egg-info/requires.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)       24 2024-05-20 13:25:19.000000 mkdocs_statblock_plugin-0.1.2/mkdocs_statblock_plugin.egg-info/top_level.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)       38 2024-05-20 13:25:19.792955 mkdocs_statblock_plugin-0.1.2/setup.cfg
--rw-r--r--   0 johannes  (1000) johannes  (1000)      919 2024-05-20 13:25:18.000000 mkdocs_statblock_plugin-0.1.2/setup.py
+drwxr-xr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-21 21:34:58.670710 mkdocs_statblock_plugin-0.1.3/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1115 2024-05-20 13:33:14.000000 mkdocs_statblock_plugin-0.1.3/LICENSE
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     3878 2024-05-21 21:34:58.670710 mkdocs_statblock_plugin-0.1.3/PKG-INFO
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     3458 2024-05-21 21:19:54.000000 mkdocs_statblock_plugin-0.1.3/README.md
+drwxr-xr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-21 21:34:58.670710 mkdocs_statblock_plugin-0.1.3/mkdocs_statblock_plugin/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2024-05-20 09:39:13.000000 mkdocs_statblock_plugin-0.1.3/mkdocs_statblock_plugin/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2136 2024-05-21 13:13:56.000000 mkdocs_statblock_plugin-0.1.3/mkdocs_statblock_plugin/mkdocs_statblock_plugin.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2423 2024-05-21 20:47:23.000000 mkdocs_statblock_plugin-0.1.3/mkdocs_statblock_plugin/statblock_handler.py
+drwxr-xr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-21 21:34:58.670710 mkdocs_statblock_plugin-0.1.3/mkdocs_statblock_plugin.egg-info/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     3878 2024-05-21 21:34:58.000000 mkdocs_statblock_plugin-0.1.3/mkdocs_statblock_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      442 2024-05-21 21:34:58.000000 mkdocs_statblock_plugin-0.1.3/mkdocs_statblock_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        1 2024-05-21 21:34:58.000000 mkdocs_statblock_plugin-0.1.3/mkdocs_statblock_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       94 2024-05-21 21:34:58.000000 mkdocs_statblock_plugin-0.1.3/mkdocs_statblock_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       21 2024-05-21 21:34:58.000000 mkdocs_statblock_plugin-0.1.3/mkdocs_statblock_plugin.egg-info/requires.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       24 2024-05-21 21:34:58.000000 mkdocs_statblock_plugin-0.1.3/mkdocs_statblock_plugin.egg-info/top_level.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       38 2024-05-21 21:34:58.670710 mkdocs_statblock_plugin-0.1.3/setup.cfg
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      919 2024-05-21 21:34:34.000000 mkdocs_statblock_plugin-0.1.3/setup.py
```

### Comparing `mkdocs_statblock_plugin-0.1.2/LICENSE` & `mkdocs_statblock_plugin-0.1.3/LICENSE`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,21 @@
-Copyright (c) 2024 johannes-z
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Copyright (c) 2024-PRESENT Johannes Zwirchmayr<https://github.com/johannes-z>
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `mkdocs_statblock_plugin-0.1.2/mkdocs_statblock_plugin/statblock_handler.py` & `mkdocs_statblock_plugin-0.1.3/mkdocs_statblock_plugin/statblock_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,41 +27,44 @@
         return default
     if label:
         return f"<b>{label}</b> {input}"
     return input
 
 
 class StatBlockHandler:
-    def __init__(self, bestiary):
+    def __init__(self, templates, templates_path, default_template, bestiary):
+        self.templates = templates
+        self.default_template = default_template
         self.bestiary = bestiary
-        self.template_env = Environment(
-            loader=FileSystemLoader(os.path.dirname(__file__))
-        )
+        self.template_env = Environment(loader=FileSystemLoader(templates_path))
         self.template_env.filters["modifier"] = modifierFilter
         self.template_env.filters["testFilter"] = testFilter
-        self.template = self.template_env.get_template("template.html")
 
     def process_statblocks(self, markdown_content):
         statblock_pattern = r"```statblock\n(.*?)```"
 
         statblocks = re.findall(statblock_pattern, markdown_content, re.DOTALL)
 
         processed_content = markdown_content
         for statblock in statblocks:
             statblock_data = self.extendMonster(yaml.safe_load(statblock))
-            rendered_statblock = self.render_template(statblock_data)
+
+            template = self.template_env.get_template(
+                statblock_data.get("template")
+                if statblock_data.get("template")
+                else self.default_template
+            )
+
+            rendered_statblock = template.render(statblock_data)
             processed_content = processed_content.replace(
                 f"```statblock\n{statblock}```", rendered_statblock
             )
 
         return processed_content
 
-    def render_template(self, data):
-        return self.template.render(data)
-
     def extendMonster(self, data):
         """Extends the monster statblock with the base monster data if it exists in the bestiary."""
         if "monster" not in data:
             return data
         monster_name = data["monster"]
         kebab_name = kebabize(monster_name)
         baseMonsterFilePath = self.bestiary[kebab_name + ".yaml"]
```

### Comparing `mkdocs_statblock_plugin-0.1.2/setup.py` & `mkdocs_statblock_plugin-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="mkdocs_statblock_plugin",
-    version="0.1.2",
+    version="0.1.3",
     description="MkDocs plugin to format YAML within statblock superfences as HTML",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/johannes-z/mkdocs-statblock-plugin.git",
     author="Johannes Zwirchmayr",
     author_email="johannes.zwirchmayr@gmail.com",
     packages=find_packages(),
```

