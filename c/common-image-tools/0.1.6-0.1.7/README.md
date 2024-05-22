# Comparing `tmp/common_image_tools-0.1.6.tar.gz` & `tmp/common_image_tools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_image_tools-0.1.6.tar", max compression
+gzip compressed data, was "common_image_tools-0.1.7.tar", max compression
```

## Comparing `common_image_tools-0.1.6.tar` & `common_image_tools-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-05-06 18:16:59.565000 common_image_tools-0.1.6/common_image_tools/__init__.py
--rw-r--r--   0        0        0     2794 2024-05-10 11:40:01.955405 common_image_tools-0.1.6/common_image_tools/conversion.py
--rw-r--r--   0        0        0     2211 2024-05-10 11:41:04.437528 common_image_tools-0.1.6/common_image_tools/operation.py
--rw-r--r--   0        0        0     5867 2024-05-10 11:42:17.895318 common_image_tools-0.1.6/common_image_tools/tool.py
--rw-r--r--   0        0        0     1359 2024-04-26 23:47:44.057023 common_image_tools-0.1.6/common_image_tools/verification.py
--rw-r--r--   0        0        0      266 2024-04-26 23:47:44.073210 common_image_tools-0.1.6/common_image_tools/visualization.py
--rw-r--r--   0        0        0      606 2024-05-10 11:44:34.865151 common_image_tools-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      832 2024-04-26 23:47:44.005195 common_image_tools-0.1.6/README.md
--rw-r--r--   0        0        0     1548 1970-01-01 00:00:00.000000 common_image_tools-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 18:16:59.565000 common_image_tools-0.1.7/common_image_tools/__init__.py
+-rw-r--r--   0        0        0     2794 2024-05-10 11:40:01.955405 common_image_tools-0.1.7/common_image_tools/conversion.py
+-rw-r--r--   0        0        0     2211 2024-05-10 11:41:04.437528 common_image_tools-0.1.7/common_image_tools/operation.py
+-rw-r--r--   0        0        0     5867 2024-05-10 11:42:17.895318 common_image_tools-0.1.7/common_image_tools/tool.py
+-rw-r--r--   0        0        0     1359 2024-04-26 23:47:44.057023 common_image_tools-0.1.7/common_image_tools/verification.py
+-rw-r--r--   0        0        0      266 2024-04-26 23:47:44.073210 common_image_tools-0.1.7/common_image_tools/visualization.py
+-rw-r--r--   0        0        0      607 2024-05-22 16:48:13.993239 common_image_tools-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      917 2024-05-15 14:28:58.459762 common_image_tools-0.1.7/README.md
+-rw-r--r--   0        0        0     1641 1970-01-01 00:00:00.000000 common_image_tools-0.1.7/PKG-INFO
```

### Comparing `common_image_tools-0.1.6/common_image_tools/conversion.py` & `common_image_tools-0.1.7/common_image_tools/conversion.py`

 * *Files identical despite different names*

### Comparing `common_image_tools-0.1.6/common_image_tools/operation.py` & `common_image_tools-0.1.7/common_image_tools/operation.py`

 * *Files identical despite different names*

### Comparing `common_image_tools-0.1.6/common_image_tools/tool.py` & `common_image_tools-0.1.7/common_image_tools/tool.py`

 * *Files identical despite different names*

### Comparing `common_image_tools-0.1.6/common_image_tools/verification.py` & `common_image_tools-0.1.7/common_image_tools/verification.py`

 * *Files identical despite different names*

### Comparing `common_image_tools-0.1.6/pyproject.toml` & `common_image_tools-0.1.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "common-image-tools"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Federico Lanzani <federico@federicolanzani.com>"]
 readme = "README.md"
 packages = [{include = "common_image_tools"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pillow = ">=9.5.0"
 opencv-python = "~4.8.0.76"
 color-transfer = "^0.1"
 scikit-image = "^0.21.0"
-dlib = "19.24.2"
+dlib = "^19.24.0"
 
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 matplotlib = "^3.7.2"
 pre-commit = "^3.5.0"
 pytest = "^8.1.1"
```

### Comparing `common_image_tools-0.1.6/README.md` & `common_image_tools-0.1.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 # Common Image Tools
 
 ## Description
+
 common_image_tools is a repository containing a curated collection of commonly used image manipulation functions for
 computer vision projects. These tools provide a set of handy functions for performing various image processing tasks,
 such as resizing, cropping, filtering, and more.
 
 ## Installation
+
 To install common_image_tools, simply run the following command:
+
 ```bash
 pip install common-image-tools
 ```
 
 ## Usage
 
 ### Tool
 
 ### Conversion
 
 ### Visualization
 
-
 ## Contributing
+
 Contributions are welcome! If you have any suggestions, improvements, or new features to add, please open an issue or
 submit a pull request. Make sure to follow the existing coding style and include appropriate tests.
 
 ## License
+
 This project is licensed under the MIT License - see the LICENSE file for details.
+
+# TODO
+
+- [ ] Change names to modules, collections of functions should be plural
```

### Comparing `common_image_tools-0.1.6/PKG-INFO` & `common_image_tools-0.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 Metadata-Version: 2.1
 Name: common-image-tools
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Federico Lanzani
 Author-email: federico@federicolanzani.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: color-transfer (>=0.1,<0.2)
-Requires-Dist: dlib (==19.24.2)
+Requires-Dist: dlib (>=19.24.0,<20.0.0)
 Requires-Dist: opencv-python (>=4.8.0.76,<4.9.0.0)
 Requires-Dist: pillow (>=9.5.0)
 Requires-Dist: scikit-image (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
 
 # Common Image Tools
 
 ## Description
+
 common_image_tools is a repository containing a curated collection of commonly used image manipulation functions for
 computer vision projects. These tools provide a set of handy functions for performing various image processing tasks,
 such as resizing, cropping, filtering, and more.
 
 ## Installation
+
 To install common_image_tools, simply run the following command:
+
 ```bash
 pip install common-image-tools
 ```
 
 ## Usage
 
 ### Tool
 
 ### Conversion
 
 ### Visualization
 
-
 ## Contributing
+
 Contributions are welcome! If you have any suggestions, improvements, or new features to add, please open an issue or
 submit a pull request. Make sure to follow the existing coding style and include appropriate tests.
 
 ## License
+
 This project is licensed under the MIT License - see the LICENSE file for details.
 
+# TODO
+
+- [ ] Change names to modules, collections of functions should be plural
```

