# Comparing `tmp/treescript_files-0.1.1.tar.gz` & `tmp/treescript_files-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treescript_files-0.1.1.tar", last modified: Wed May  1 14:54:33 2024, max compression
+gzip compressed data, was "treescript_files-0.2.tar", last modified: Wed May 22 16:13:25 2024, max compression
```

## Comparing `treescript_files-0.1.1.tar` & `treescript_files-0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:54:33.921250 treescript_files-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 14:54:22.000000 treescript_files-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-01 14:54:33.921250 treescript_files-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-01 14:54:22.000000 treescript_files-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:54:22.000000 treescript_files-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:54:33.921250 treescript_files-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-01 14:54:22.000000 treescript_files-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:54:33.917250 treescript_files-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-01 14:54:22.000000 treescript_files-0.1.1/test/test_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-05-01 14:54:22.000000 treescript_files-0.1.1/test/test_line_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-01 14:54:22.000000 treescript_files-0.1.1/test/test_path_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-01 14:54:22.000000 treescript_files-0.1.1/test/test_tree_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:54:33.921250 treescript_files-0.1.1/treescript_files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:54:22.000000 treescript_files-0.1.1/treescript_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-01 14:54:22.000000 treescript_files-0.1.1/treescript_files/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-01 14:54:22.000000 treescript_files-0.1.1/treescript_files/argument_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-01 14:54:22.000000 treescript_files-0.1.1/treescript_files/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-01 14:54:22.000000 treescript_files-0.1.1/treescript_files/file_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-01 14:54:22.000000 treescript_files-0.1.1/treescript_files/input_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-01 14:54:22.000000 treescript_files-0.1.1/treescript_files/line_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-01 14:54:22.000000 treescript_files-0.1.1/treescript_files/path_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-01 14:54:22.000000 treescript_files-0.1.1/treescript_files/string_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-01 14:54:22.000000 treescript_files-0.1.1/treescript_files/tree_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-01 14:54:22.000000 treescript_files-0.1.1/treescript_files/tree_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:54:33.921250 treescript_files-0.1.1/treescript_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-01 14:54:33.000000 treescript_files-0.1.1/treescript_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-01 14:54:33.000000 treescript_files-0.1.1/treescript_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:54:33.000000 treescript_files-0.1.1/treescript_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-01 14:54:33.000000 treescript_files-0.1.1/treescript_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 14:54:33.000000 treescript_files-0.1.1/treescript_files.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:25.957641 treescript_files-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 16:13:15.000000 treescript_files-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-22 16:13:25.957641 treescript_files-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-22 16:13:15.000000 treescript_files-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:15.000000 treescript_files-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:13:25.957641 treescript_files-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-22 16:13:15.000000 treescript_files-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:25.957641 treescript_files-0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-22 16:13:15.000000 treescript_files-0.2/test/test_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-05-22 16:13:15.000000 treescript_files-0.2/test/test_line_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-22 16:13:15.000000 treescript_files-0.2/test/test_path_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-22 16:13:15.000000 treescript_files-0.2/test/test_tree_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:25.957641 treescript_files-0.2/treescript_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-22 16:13:15.000000 treescript_files-0.2/treescript_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-22 16:13:15.000000 treescript_files-0.2/treescript_files/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-22 16:13:15.000000 treescript_files-0.2/treescript_files/argument_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-22 16:13:15.000000 treescript_files-0.2/treescript_files/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-22 16:13:15.000000 treescript_files-0.2/treescript_files/file_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-22 16:13:15.000000 treescript_files-0.2/treescript_files/input_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-22 16:13:15.000000 treescript_files-0.2/treescript_files/line_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-22 16:13:15.000000 treescript_files-0.2/treescript_files/path_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-22 16:13:15.000000 treescript_files-0.2/treescript_files/string_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-22 16:13:15.000000 treescript_files-0.2/treescript_files/tree_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-22 16:13:15.000000 treescript_files-0.2/treescript_files/tree_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:25.957641 treescript_files-0.2/treescript_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-22 16:13:25.000000 treescript_files-0.2/treescript_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-22 16:13:25.000000 treescript_files-0.2/treescript_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:13:25.000000 treescript_files-0.2/treescript_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-22 16:13:25.000000 treescript_files-0.2/treescript_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 16:13:25.000000 treescript_files-0.2/treescript_files.egg-info/top_level.txt
```

### Comparing `treescript_files-0.1.1/LICENSE` & `treescript_files-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `treescript_files-0.1.1/PKG-INFO` & `treescript_files-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treescript-files
-Version: 0.1.1
+Version: 0.2
 Summary: Obtains the relative path of all files in the TreeScript.
 Author: DK96-OS
 License: GPLv3
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `treescript_files-0.1.1/README.md` & `treescript_files-0.2/README.md`

 * *Files identical despite different names*

### Comparing `treescript_files-0.1.1/setup.py` & `treescript_files-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup Package Configuration
 """
 from setuptools import setup, find_packages
 
 
 setup(
     name="treescript-files",
-    version="0.1.1",
+    version="0.2",
     description="Obtains the relative path of all files in the TreeScript.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="DK96-OS",
     #url="https://github.com/DK96-OS/treescript-files/",
     project_urls={
         #"Issues": "https://github.com/DK96-OS/treescript-files/issues",
```

### Comparing `treescript_files-0.1.1/test/test_line_reader.py` & `treescript_files-0.2/test/test_line_reader.py`

 * *Files identical despite different names*

### Comparing `treescript_files-0.1.1/test/test_path_stack.py` & `treescript_files-0.2/test/test_path_stack.py`

 * *Files identical despite different names*

### Comparing `treescript_files-0.1.1/test/test_tree_reader.py` & `treescript_files-0.2/test/test_tree_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Testing Tree Reader and Process Input Data Method
 """
 import pytest
+
 from treescript_files.input_data import InputData
 from treescript_files.tree_reader import process_input_data
 
 
 def test_process_input_data_single_file():
     input_data = InputData(
         tree_input='src/\n  file.py',
@@ -32,15 +33,15 @@
     )
     result = list(process_input_data(input_data))
     assert len(result) == 2
     assert result[0] == 'src/file.py'
     assert result[1] == 'src/file2.py'
 
 
-def test_process_input_data_two_files():
+def test_process_input_data_two_files_parent_path():
     input_data = InputData(
         tree_input='src/\n  file.py\n  file2.py',
         parent_path='module/'
     )
     result = list(process_input_data(input_data))
     assert len(result) == 2
     assert result[0] == 'module/src/file.py'
```

### Comparing `treescript_files-0.1.1/treescript_files/__main__.py` & `treescript_files-0.2/treescript_files/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/python
 from sys import argv, path
 
+from treescript_files import ts_files
 from treescript_files.argument_parser import parse_arguments
 from treescript_files.input_data import validate_arguments
-from treescript_files.tree_reader import process_input_data
 
 
 def main():
     input_data = validate_arguments(
         parse_arguments(argv[1:])
     )
-    for file in process_input_data(input_data):
-        print(file)
+    output_data = ts_files(input_data)
+    print(output_data)
 
 
 if __name__ == "__main__":
     from pathlib import Path
     # Get the directory of the current file (__file__ is the path to the script being executed)
     current_directory = Path(__file__).resolve().parent.parent
     # Add the directory to sys.path
```

### Comparing `treescript_files-0.1.1/treescript_files/argument_data.py` & `treescript_files-0.2/treescript_files/argument_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,11 +13,13 @@
 class ArgumentData:
     """
     The syntactically valid arguments recevied by the Program.
 
     Fields:
     - tree_file (str): The file containing the Tree.
     - parent_path (str | None): The parent path to prefix files with.
+    - separator (str): The separator to use in the program output.
     """
 
     tree_file: str
     parent_path: str | None
+    separator: str
```

### Comparing `treescript_files-0.1.1/treescript_files/file_validation.py` & `treescript_files-0.2/treescript_files/file_validation.py`

 * *Files identical despite different names*

### Comparing `treescript_files-0.1.1/treescript_files/input_data.py` & `treescript_files-0.2/treescript_files/input_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 @dataclass(frozen=True)
 class InputData:
     """A Data Class Containing Program Input.
 
     Fields:
     - tree_input (str): The Tree Input to the program.
     - parent_path (str | None): The Parent Path to prefix, or None.
+    - separator (str): The separator between elements in the program output.
     """
 
     tree_input: str
     parent_path: str | None
+    separator : str = '\n'
 
     def get_tree_data(self) -> Generator[TreeData, None, None]:
         """
         Initializes a Generator for processing the Tree Input.
             See line_reader module for more details.
 
         Returns:
@@ -33,9 +35,10 @@
 
 
 def validate_arguments(argument_data: ArgumentData) -> InputData:
     """Validate ArgumentData and return InputData.
     """
     return InputData(
         tree_input=validate_input_file(argument_data.tree_file),
-        parent_path=argument_data.parent_path
+        parent_path=argument_data.parent_path,
+        separator=argument_data.separator,
     )
```

### Comparing `treescript_files-0.1.1/treescript_files/line_reader.py` & `treescript_files-0.2/treescript_files/line_reader.py`

 * *Files identical despite different names*

### Comparing `treescript_files-0.1.1/treescript_files/path_stack.py` & `treescript_files-0.2/treescript_files/path_stack.py`

 * *Files identical despite different names*

### Comparing `treescript_files-0.1.1/treescript_files/string_validation.py` & `treescript_files-0.2/treescript_files/string_validation.py`

 * *Files identical despite different names*

### Comparing `treescript_files-0.1.1/treescript_files/tree_reader.py` & `treescript_files-0.2/treescript_files/tree_reader.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 from .tree_data import TreeData
 
 
 def process_input_data(
     input_data: InputData,
 ) -> Generator[str, None, None]:
     """Process the Input Data and set-up file path generators.
+
+    Parameters:
+    - input_data (InputData): The program input data.
+
+    Returns:
+    Generator[str] - Yields the strings.
     """
     file_generator = _process_tree_data(input_data.get_tree_data())
     if (parent := input_data.parent_path) is not None:
         file_generator = _prefix_parent(parent, file_generator)
     return file_generator
```

### Comparing `treescript_files-0.1.1/treescript_files.egg-info/PKG-INFO` & `treescript_files-0.2/treescript_files.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treescript-files
-Version: 0.1.1
+Version: 0.2
 Summary: Obtains the relative path of all files in the TreeScript.
 Author: DK96-OS
 License: GPLv3
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `treescript_files-0.1.1/treescript_files.egg-info/SOURCES.txt` & `treescript_files-0.2/treescript_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

