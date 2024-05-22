# Comparing `tmp/proconfig-0.1.5.tar.gz` & `tmp/proconfig-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proconfig-0.1.5.tar", last modified: Mon May 20 09:36:25 2024, max compression
+gzip compressed data, was "proconfig-0.1.6.tar", last modified: Wed May 22 02:49:43 2024, max compression
```

## Comparing `proconfig-0.1.5.tar` & `proconfig-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 I530319    (501) staff       (20)        0 2024-05-20 09:36:25.498657 proconfig-0.1.5/
--rw-r--r--   0 I530319    (501) staff       (20)     2670 2024-05-20 09:36:25.498164 proconfig-0.1.5/PKG-INFO
--rw-r--r--   0 I530319    (501) staff       (20)     2157 2024-05-10 15:38:45.000000 proconfig-0.1.5/README.md
-drwxr-xr-x   0 I530319    (501) staff       (20)        0 2024-05-20 09:36:25.493480 proconfig-0.1.5/proconfig/
--rw-r--r--   0 I530319    (501) staff       (20)     1787 2024-05-20 08:41:05.000000 proconfig-0.1.5/proconfig/__init__.py
--rw-r--r--   0 I530319    (501) staff       (20)       22 2024-05-20 09:36:07.000000 proconfig-0.1.5/proconfig/__version__.py
--rw-r--r--   0 I530319    (501) staff       (20)     5771 2024-05-20 09:34:19.000000 proconfig-0.1.5/proconfig/cli.py
-drwxr-xr-x   0 I530319    (501) staff       (20)        0 2024-05-20 09:36:25.497798 proconfig-0.1.5/proconfig.egg-info/
--rw-r--r--   0 I530319    (501) staff       (20)     2670 2024-05-20 09:36:25.000000 proconfig-0.1.5/proconfig.egg-info/PKG-INFO
--rw-r--r--   0 I530319    (501) staff       (20)      282 2024-05-20 09:36:25.000000 proconfig-0.1.5/proconfig.egg-info/SOURCES.txt
--rw-r--r--   0 I530319    (501) staff       (20)        1 2024-05-20 09:36:25.000000 proconfig-0.1.5/proconfig.egg-info/dependency_links.txt
--rw-r--r--   0 I530319    (501) staff       (20)       42 2024-05-20 09:36:25.000000 proconfig-0.1.5/proconfig.egg-info/entry_points.txt
--rw-r--r--   0 I530319    (501) staff       (20)       25 2024-05-20 09:36:25.000000 proconfig-0.1.5/proconfig.egg-info/requires.txt
--rw-r--r--   0 I530319    (501) staff       (20)       10 2024-05-20 09:36:25.000000 proconfig-0.1.5/proconfig.egg-info/top_level.txt
--rw-r--r--   0 I530319    (501) staff       (20)       38 2024-05-20 09:36:25.498709 proconfig-0.1.5/setup.cfg
--rw-r--r--   0 I530319    (501) staff       (20)      829 2024-05-20 08:30:45.000000 proconfig-0.1.5/setup.py
+drwxr-xr-x   0 I530319    (501) staff       (20)        0 2024-05-22 02:49:43.544701 proconfig-0.1.6/
+-rw-r--r--   0 I530319    (501) staff       (20)     2717 2024-05-22 02:49:43.544286 proconfig-0.1.6/PKG-INFO
+-rw-r--r--   0 I530319    (501) staff       (20)     2157 2024-05-10 15:38:45.000000 proconfig-0.1.6/README.md
+drwxr-xr-x   0 I530319    (501) staff       (20)        0 2024-05-22 02:49:43.538239 proconfig-0.1.6/proconfig/
+-rw-r--r--   0 I530319    (501) staff       (20)    10979 2024-05-21 12:01:10.000000 proconfig-0.1.6/proconfig/__init__.py
+-rw-r--r--   0 I530319    (501) staff       (20)       22 2024-05-22 02:37:58.000000 proconfig-0.1.6/proconfig/__version__.py
+-rw-r--r--   0 I530319    (501) staff       (20)     6646 2024-05-22 02:48:41.000000 proconfig-0.1.6/proconfig/cli.py
+drwxr-xr-x   0 I530319    (501) staff       (20)        0 2024-05-22 02:49:43.543922 proconfig-0.1.6/proconfig.egg-info/
+-rw-r--r--   0 I530319    (501) staff       (20)     2717 2024-05-22 02:49:43.000000 proconfig-0.1.6/proconfig.egg-info/PKG-INFO
+-rw-r--r--   0 I530319    (501) staff       (20)      282 2024-05-22 02:49:43.000000 proconfig-0.1.6/proconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 I530319    (501) staff       (20)        1 2024-05-22 02:49:43.000000 proconfig-0.1.6/proconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 I530319    (501) staff       (20)       42 2024-05-22 02:49:43.000000 proconfig-0.1.6/proconfig.egg-info/entry_points.txt
+-rw-r--r--   0 I530319    (501) staff       (20)       42 2024-05-22 02:49:43.000000 proconfig-0.1.6/proconfig.egg-info/requires.txt
+-rw-r--r--   0 I530319    (501) staff       (20)       10 2024-05-22 02:49:43.000000 proconfig-0.1.6/proconfig.egg-info/top_level.txt
+-rw-r--r--   0 I530319    (501) staff       (20)       38 2024-05-22 02:49:43.544756 proconfig-0.1.6/setup.cfg
+-rw-r--r--   0 I530319    (501) staff       (20)      868 2024-05-22 02:39:07.000000 proconfig-0.1.6/setup.py
```

### Comparing `proconfig-0.1.5/PKG-INFO` & `proconfig-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: proconfig
-Version: 0.1.5
+Version: 0.1.6
 Summary: A CLI tool for simplify MyShell PorConfig programming.
 Home-page: https://github.com/cybernagle/proconfig-generator
 Author: cybernagle
 Author-email: zhang.nagle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: tabulate
 Requires-Dist: termcolor
+Requires-Dist: jsonschema
+Requires-Dist: click
 
 # MyShell ProConfig Generator
 
 Welcome to the MyShell ProConfig Generator project! This command-line interface (CLI) tool is designed to streamline the creation of your custom MyShell configurations.
 
 ## Issues with Current MyShell Configurations
 Currently, users face several challenges with MyShell configurations:
```

### Comparing `proconfig-0.1.5/README.md` & `proconfig-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `proconfig-0.1.5/proconfig/cli.py` & `proconfig-0.1.6/proconfig/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 
 import os
 import sys
 import json
 import yaml
 import click
 
+import jsonschema
+from jsonschema import validate
 from tabulate import tabulate
 from termcolor import colored
 
 from . import MAIN_YAML_CONTENT, HOME_PAGE_STATE_CONTENT, QUESTIONS_JSON_CONTENT, LEVEL1_JS_CONTENT
+from . import schema
 
 # class to implement a custom YAML loader
 class Loader(yaml.SafeLoader):
     def __init__(self, stream):
         self._root = os.path.split(stream.name)[0]
         self._headers = ['state', 'inputs', 'outputs', 'transitions', 'render', 'tasks']
         self._state = []
@@ -30,56 +33,85 @@
             if filename.endswith('.yaml') or filename.endswith('.yml'):
                 file_path = os.path.join(full_directory_path, filename)
                 with open(file_path, 'r') as f:
                     # 合并yaml文件内容
                     file_data = yaml.load(f, Loader=yaml.FullLoader)
                     if isinstance(file_data, dict) and file_data:
                         data.update(file_data)
-                        self.handle_stage(file_data)
                     elif isinstance(file_data, list):
                         data[filename] = file_data
         return data
 
-    def handle_stage(self, stages):
-        for state_name in list(stages.keys()):
-            state = stages[state_name]
-            self.update_fields(state_name ,state)
 
     def oneline(self, node):
         file_path = self.construct_scalar(node)
         if not os.path.exists(file_path):
             raise FileNotFoundError(f"File {file_path} not found")
 
-        # 如果是 YAML 文件，合并内容
         with open(file_path, 'r') as f:
             return f.read()#.replace('\\n', '\n')
 
-    def update_fields(self, state_name ,state_data):
+
+    def print_table(self, data):
+        headers_upper = [header.upper() for header in self._headers]
+        colalign = ["right"] * len(headers_upper)
+        print(tabulate(data, headers=headers_upper, tablefmt='plain', colalign=colalign),file=sys.stderr)
+
+Loader.add_constructor('!include', Loader.include)
+Loader.add_constructor('!oneline', Loader.oneline)
+
+def visualize(states):
+    headers = ['state', 'inputs', 'outputs', 'transitions', 'render', 'tasks']
+    data = []
+    for state_name in list(states.keys()):
         single_state = []
-        for header in self._headers:
+        state_data = states[state_name]
+
+        for header in headers:
             if header in state_data:
                 single_state.append(colored('Yes', 'green'))
             elif header == "state":
                 single_state.append(colored(state_name, 'yellow'))
             else:
                 single_state.append(colored('No', 'red'))
+        data += [single_state]
 
-        self._state += [single_state]
+    headers_upper = [header.upper() for header in headers]
+    colalign = ["right"] * len(headers_upper)
+    print(tabulate(data, headers=headers_upper, tablefmt='plain', colalign=colalign),file=sys.stderr)
 
-    def print_table(self, data):
-        headers_upper = [header.upper() for header in self._headers]
-        colalign = ["right"] * len(headers_upper)
-        print(tabulate(data, headers=headers_upper, tablefmt='plain', colalign=colalign),file=sys.stderr)
+def load_file(file_path):
+    _, file_extension = os.path.splitext(file_path)
 
-    def __del__(self):
-        if self._state:
-            self.print_table(self._state)
+    try:
+        if file_extension.lower() == '.json':
+            with open(file_path, 'r', encoding='utf-8') as f:
+                return json.load(f)
+        elif file_extension.lower() in ['.yaml', '.yml']:
+            with open(file_path, 'r', encoding='utf-8') as f:
+                return yaml.load(f, Loader)
+        else:
+            raise click.UsageError(f"Unsupported file extension: {file_extension}")
 
-Loader.add_constructor('!include', Loader.include)
-Loader.add_constructor('!oneline', Loader.oneline)
+    except (json.JSONDecodeError, yaml.YAMLError) as e:
+        raise click.UsageError(f"Invalid file format: {e}")
+
+def validate_proconfig(json_data):
+    try:
+        validate(instance=json_data, schema=schema)
+    except jsonschema.ValidationError as e:
+        error_message = (
+            f"Validation error: {e.message}\n"
+            f"Path to error: {list(e.path)}\n"
+            f"Schema path: {list(e.schema_path)}"
+        )
+        raise click.UsageError(f"Invalid JSON content: {error_message}")
+    print("DATA validation successful: The provided ProConfig Code is valid.")
+    if 'states' in json_data:
+        visualize(json_data['states'])
 
 def create_project_structure():
     """Initialize the project structure."""
     current_dir = os.getcwd()
 
     if (os.path.exists(os.path.join(current_dir, 'main.yaml')) or
         os.path.exists(os.path.join(current_dir, 'state')) or
@@ -103,61 +135,50 @@
     with open(os.path.join(current_dir, 'code', 'level1.js'), 'w') as f:
         f.write(LEVEL1_JS_CONTENT)
 
     click.echo("Project structure initialized successfully.")
 
 from .__version__ import __version__
 
-@click.group()
-@click.version_option(__version__, '-v', '--version', message='%(version)s')
-def cli():
-    pass
 
 @click.group(invoke_without_command=True)
+@click.version_option(__version__, '-v', '--version', message='%(version)s')
 @click.pass_context
 def cli(ctx):
     if ctx.invoked_subcommand is None:
-        # If no subcommand is invoked, call the default command
-        ctx.invoke(encode)
+        click.echo(ctx.get_help())
 
 @cli.command()
 @click.argument('json_file', type=click.File('r'))
-@click.option('--output', '-o', type=click.File('w'), default='-',
-              help='Output file path. Defaults to stdout.')
+@click.option('--output', '-o', type=click.File('w'), default='output.yaml',
+              help='Output file path. Defaults to output.yaml.')
 def decode(json_file, output):
     """Convert JSON to YAML."""
-    try:
-        json_data = json.load(json_file)
-    except json.JSONDecodeError:
-        raise click.UsageError(f"Invalid JSON format in file: {json_file.name}")
-
+    json_data = load_file(json_file.name)
     yaml.dump(json_data, output, default_flow_style=False)
 
+    validate_proconfig(json_data)
 
 @cli.command()
 @click.argument('yaml_file', type=click.File('r'), default='main.yaml')
-@click.option('--output', '-o', type=click.File('w'), default='-',
-              help='Output file path. Defaults to stdout.')
+@click.option('--output', '-o', type=click.File('w'), default='output.json',
+              help='Output file path. Defaults to output.json.')
 def encode(yaml_file, output):
     """Convert YAML to JSON."""
-    try:
-        yaml_data = yaml.load(yaml_file, Loader)
-    except yaml.YAMLError:
-        raise click.UsageError(f"Invalid YAML format in file: {yaml_file.name}")
-
+    yaml_data = load_file(yaml_file.name)
     json.dump(yaml_data, output)
 
+    validate_proconfig(yaml_data)
+
 @cli.command()
 @click.argument('yaml_file', type=click.File('r'))
 def check(yaml_file):
     """Check the state for missing part."""
-    try:
-        yaml_data = yaml.load(yaml_file, Loader)
-    except yaml.YAMLError:
-        raise click.UsageError(f"Invalid YAML format in file: {yaml_file.name}")
+    yaml_data = load_file(yaml_file.name)
+    validate_proconfig(yaml_data)
 
 @cli.command()
 def init():
     """Init a whole simple project."""
     create_project_structure()
 
 if __name__ == '__main__':
```

### Comparing `proconfig-0.1.5/proconfig.egg-info/PKG-INFO` & `proconfig-0.1.6/proconfig.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: proconfig
-Version: 0.1.5
+Version: 0.1.6
 Summary: A CLI tool for simplify MyShell PorConfig programming.
 Home-page: https://github.com/cybernagle/proconfig-generator
 Author: cybernagle
 Author-email: zhang.nagle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: tabulate
 Requires-Dist: termcolor
+Requires-Dist: jsonschema
+Requires-Dist: click
 
 # MyShell ProConfig Generator
 
 Welcome to the MyShell ProConfig Generator project! This command-line interface (CLI) tool is designed to streamline the creation of your custom MyShell configurations.
 
 ## Issues with Current MyShell Configurations
 Currently, users face several challenges with MyShell configurations:
```

### Comparing `proconfig-0.1.5/setup.py` & `proconfig-0.1.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='proconfig',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'click',
         "tabulate",
         "termcolor",
+        "jsonschema",
+        "click",
     ],
     entry_points='''
         [console_scripts]
         pcc=proconfig.cli:cli
     ''',
     author='cybernagle',
     author_email='zhang.nagle@gmail.com',
```

