# Comparing `tmp/pythontk-0.7.8.tar.gz` & `tmp/pythontk-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythontk-0.7.8.tar", last modified: Mon Dec 11 21:48:35 2023, max compression
+gzip compressed data, was "pythontk-0.7.9.tar", last modified: Mon Dec 11 22:24:15 2023, max compression
```

## Comparing `pythontk-0.7.8.tar` & `pythontk-0.7.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-12-11 21:48:35.766021 pythontk-0.7.8/
--rw-rw-rw-   0        0        0     1093 2023-09-06 12:43:43.000000 pythontk-0.7.8/LICENSE
--rw-rw-rw-   0        0        0     2027 2023-12-11 21:48:35.765022 pythontk-0.7.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-12-11 21:48:35.727138 pythontk-0.7.8/pythontk/
--rw-rw-rw-   0        0        0     2294 2023-12-11 21:48:29.000000 pythontk-0.7.8/pythontk/__init__.py
--rw-rw-rw-   0        0        0    12335 2023-09-06 12:43:43.000000 pythontk-0.7.8/pythontk/core_utils.py
--rw-rw-rw-   0        0        0    34495 2023-12-11 21:05:06.000000 pythontk-0.7.8/pythontk/file_utils.py
--rw-rw-rw-   0        0        0    24606 2023-12-03 03:58:25.000000 pythontk-0.7.8/pythontk/img_utils.py
--rw-rw-rw-   0        0        0    15998 2023-10-23 14:26:21.000000 pythontk-0.7.8/pythontk/iter_utils.py
--rw-rw-rw-   0        0        0    18963 2023-09-06 12:43:43.000000 pythontk-0.7.8/pythontk/math_utils.py
--rw-rw-rw-   0        0        0    26241 2023-09-06 12:43:43.000000 pythontk-0.7.8/pythontk/str_utils.py
-drwxrwxrwx   0        0        0        0 2023-12-11 21:48:35.764023 pythontk-0.7.8/pythontk.egg-info/
--rw-rw-rw-   0        0        0     2027 2023-12-11 21:48:35.000000 pythontk-0.7.8/pythontk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-12-11 21:48:35.000000 pythontk-0.7.8/pythontk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-11 21:48:35.000000 pythontk-0.7.8/pythontk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-12-11 21:48:35.000000 pythontk-0.7.8/pythontk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-12-11 21:48:35.000000 pythontk-0.7.8/pythontk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-11 21:48:35.766021 pythontk-0.7.8/setup.cfg
--rw-rw-rw-   0        0        0     1506 2023-12-11 21:48:12.000000 pythontk-0.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:24:15.137692 pythontk-0.7.9/
+-rw-rw-rw-   0        0        0     1093 2023-09-06 12:43:43.000000 pythontk-0.7.9/LICENSE
+-rw-rw-rw-   0        0        0     2027 2023-12-11 22:24:15.136687 pythontk-0.7.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-12-11 22:24:15.105036 pythontk-0.7.9/pythontk/
+-rw-rw-rw-   0        0        0     2294 2023-12-11 22:24:11.000000 pythontk-0.7.9/pythontk/__init__.py
+-rw-rw-rw-   0        0        0    12335 2023-09-06 12:43:43.000000 pythontk-0.7.9/pythontk/core_utils.py
+-rw-rw-rw-   0        0        0    34743 2023-12-11 22:22:34.000000 pythontk-0.7.9/pythontk/file_utils.py
+-rw-rw-rw-   0        0        0    24606 2023-12-03 03:58:25.000000 pythontk-0.7.9/pythontk/img_utils.py
+-rw-rw-rw-   0        0        0    15998 2023-10-23 14:26:21.000000 pythontk-0.7.9/pythontk/iter_utils.py
+-rw-rw-rw-   0        0        0    18963 2023-09-06 12:43:43.000000 pythontk-0.7.9/pythontk/math_utils.py
+-rw-rw-rw-   0        0        0    26241 2023-09-06 12:43:43.000000 pythontk-0.7.9/pythontk/str_utils.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:24:15.135577 pythontk-0.7.9/pythontk.egg-info/
+-rw-rw-rw-   0        0        0     2027 2023-12-11 22:24:15.000000 pythontk-0.7.9/pythontk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-12-11 22:24:15.000000 pythontk-0.7.9/pythontk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-11 22:24:15.000000 pythontk-0.7.9/pythontk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-12-11 22:24:15.000000 pythontk-0.7.9/pythontk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-12-11 22:24:15.000000 pythontk-0.7.9/pythontk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-11 22:24:15.137692 pythontk-0.7.9/setup.cfg
+-rw-rw-rw-   0        0        0     1374 2023-12-11 22:13:20.000000 pythontk-0.7.9/setup.py
```

### Comparing `pythontk-0.7.8/LICENSE` & `pythontk-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pythontk-0.7.8/PKG-INFO` & `pythontk-0.7.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pythontk
-Version: 0.7.8
+Version: 0.7.9
 Summary: *pythontk is a collection of backend utilities for Python.*
 Home-page: https://github.com/m3trik/pythontk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.24.1
 Requires-Dist: Pillow==9.3.0
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![Version](https://img.shields.io/badge/Version-0.7.8-blue.svg)](https://pypi.org/project/pythontk/)
+[![Version](https://img.shields.io/badge/Version-0.7.9-blue.svg)](https://pypi.org/project/pythontk/)
 [![CoreUtils Tests](https://img.shields.io/badge/CoreUtils-Passing-brightgreen.svg)](../test/ptk_test.py#CoreUtilsTest)
 [![FileUtils Tests](https://img.shields.io/badge/FileUtils-Passing-brightgreen.svg)](../test/ptk_test.py#FileUtilsTest)
 [![ImgUtils Tests](https://img.shields.io/badge/ImgUtils-Passing-brightgreen.svg)](../test/ptk_test.py#ImgUtilsTest)
 [![MathUtils Tests](https://img.shields.io/badge/MathUtils-Passing-brightgreen.svg)](../test/ptk_test.py#MathUtilsTest)
 [![IterUtils Tests](https://img.shields.io/badge/IterUtils-Passing-brightgreen.svg)](../test/ptk_test.py#IterUtilsTest)
 [![StrUtils Tests](https://img.shields.io/badge/StrUtils-Passing-brightgreen.svg)](../test/ptk_test.py#StrUtilsTest)
```

### Comparing `pythontk-0.7.8/pythontk/__init__.py` & `pythontk-0.7.9/pythontk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # !/usr/bin/python
 # coding=utf-8
 import inspect
 import importlib
 import pkgutil
 
 __package__ = "pythontk"
-__version__ = "0.7.8"
+__version__ = "0.7.9"
 
 CLASS_TO_MODULE = {}
 METHOD_TO_MODULE = {}
 CLASS_METHOD_TO_MODULE = {}
 IMPORTED_MODULES = {}
```

### Comparing `pythontk-0.7.8/pythontk/core_utils.py` & `pythontk-0.7.9/pythontk/core_utils.py`

 * *Files identical despite different names*

### Comparing `pythontk-0.7.8/pythontk/file_utils.py` & `pythontk-0.7.9/pythontk/file_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -762,15 +762,15 @@
         cls.write_to_file(filepath, lines)
         if not version:
             print(f"Error: No version found in {filepath}")
         return version
 
     @staticmethod
     def update_requirements(file_path=None):
-        """Update the requirements.txt file with the current versions of the packages.
+        """Update the requirements.txt file with the current versions of packages.
 
         Parameters:
             file_path (str): Path to the requirements.txt file. Defaults to the caller's directory.
                              If a relative path is given, it's relative to the caller's directory.
         """
         import inspect
         import pkg_resources
@@ -782,15 +782,15 @@
 
         if file_path is None:
             file_path = os.path.join(caller_dir, "requirements.txt")
         else:
             # Resolve relative paths relative to the caller's directory
             file_path = os.path.abspath(os.path.join(caller_dir, file_path))
 
-        required_packages = []
+        updated_lines = []
 
         try:
             # Read the existing requirements.txt
             with open(file_path, "r") as file:
                 lines = file.readlines()
 
             for line in lines:
@@ -800,22 +800,27 @@
 
                 # Extract package name
                 package_name = line.strip().split("==")[0]
 
                 try:
                     # Get the current version of the package
                     version = pkg_resources.get_distribution(package_name).version
-                    required_packages.append(f"{package_name}=={version}")
+                    updated_lines.append(f"{package_name}=={version}\n")
                 except Exception as e:
                     print(f"Error updating version for {package_name}: {e}")
+                    updated_lines.append(line)
+
+            # Write the updated requirements back to the file
+            with open(file_path, "w") as file:
+                file.writelines(updated_lines)
 
         except FileNotFoundError:
             print(f"File not found: {file_path}")
 
-        return required_packages
+        return updated_lines  # Return the updated package requirements as a list
 
 
 # --------------------------------------------------------------------------------------------
 
 if __name__ == "__main__":
     pass
```

### Comparing `pythontk-0.7.8/pythontk/img_utils.py` & `pythontk-0.7.9/pythontk/img_utils.py`

 * *Files identical despite different names*

### Comparing `pythontk-0.7.8/pythontk/iter_utils.py` & `pythontk-0.7.9/pythontk/iter_utils.py`

 * *Files identical despite different names*

### Comparing `pythontk-0.7.8/pythontk/math_utils.py` & `pythontk-0.7.9/pythontk/math_utils.py`

 * *Files identical despite different names*

### Comparing `pythontk-0.7.8/pythontk/str_utils.py` & `pythontk-0.7.9/pythontk/str_utils.py`

 * *Files identical despite different names*

### Comparing `pythontk-0.7.8/pythontk.egg-info/PKG-INFO` & `pythontk-0.7.9/pythontk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pythontk
-Version: 0.7.8
+Version: 0.7.9
 Summary: *pythontk is a collection of backend utilities for Python.*
 Home-page: https://github.com/m3trik/pythontk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.24.1
 Requires-Dist: Pillow==9.3.0
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![Version](https://img.shields.io/badge/Version-0.7.8-blue.svg)](https://pypi.org/project/pythontk/)
+[![Version](https://img.shields.io/badge/Version-0.7.9-blue.svg)](https://pypi.org/project/pythontk/)
 [![CoreUtils Tests](https://img.shields.io/badge/CoreUtils-Passing-brightgreen.svg)](../test/ptk_test.py#CoreUtilsTest)
 [![FileUtils Tests](https://img.shields.io/badge/FileUtils-Passing-brightgreen.svg)](../test/ptk_test.py#FileUtilsTest)
 [![ImgUtils Tests](https://img.shields.io/badge/ImgUtils-Passing-brightgreen.svg)](../test/ptk_test.py#ImgUtilsTest)
 [![MathUtils Tests](https://img.shields.io/badge/MathUtils-Passing-brightgreen.svg)](../test/ptk_test.py#MathUtilsTest)
 [![IterUtils Tests](https://img.shields.io/badge/IterUtils-Passing-brightgreen.svg)](../test/ptk_test.py#IterUtilsTest)
 [![StrUtils Tests](https://img.shields.io/badge/StrUtils-Passing-brightgreen.svg)](../test/ptk_test.py#StrUtilsTest)
```

