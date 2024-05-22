# Comparing `tmp/colorcompass-1.2.1.tar.gz` & `tmp/colorcompass-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorcompass-1.2.1.tar", last modified: Wed Oct 18 11:32:41 2023, max compression
+gzip compressed data, was "colorcompass-1.2.3.tar", last modified: Wed May 22 02:01:50 2024, max compression
```

## Comparing `colorcompass-1.2.1.tar` & `colorcompass-1.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nicolasagustinaguirrecampi   (501) staff       (20)        0 2023-10-18 11:32:41.596456 colorcompass-1.2.1/
--rw-r--r--   0 nicolasagustinaguirrecampi   (501) staff       (20)     1077 2023-10-13 13:14:37.000000 colorcompass-1.2.1/LICENSE.md
--rw-r--r--   0 nicolasagustinaguirrecampi   (501) staff       (20)     3861 2023-10-18 11:32:41.596174 colorcompass-1.2.1/PKG-INFO
--rw-r--r--   0 nicolasagustinaguirrecampi   (501) staff       (20)     3251 2023-10-18 11:22:34.000000 colorcompass-1.2.1/README.md
-drwxr-xr-x   0 nicolasagustinaguirrecampi   (501) staff       (20)        0 2023-10-18 11:32:41.591591 colorcompass-1.2.1/colorcompass/
--rw-r--r--   0 nicolasagustinaguirrecampi   (501) staff       (20)       41 2023-10-17 18:30:53.000000 colorcompass-1.2.1/colorcompass/__init__.py
--rw-r--r--   0 nicolasagustinaguirrecampi   (501) staff       (20)     2628 2023-10-17 19:19:45.000000 colorcompass-1.2.1/colorcompass/color_compass.py
--rw-r--r--   0 nicolasagustinaguirrecampi   (501) staff       (20)    31533 2023-10-17 19:19:31.000000 colorcompass-1.2.1/colorcompass/color_dictionary.py
-drwxr-xr-x   0 nicolasagustinaguirrecampi   (501) staff       (20)        0 2023-10-18 11:32:41.595234 colorcompass-1.2.1/colorcompass.egg-info/
--rw-r--r--   0 nicolasagustinaguirrecampi   (501) staff       (20)     3861 2023-10-18 11:32:41.000000 colorcompass-1.2.1/colorcompass.egg-info/PKG-INFO
--rw-r--r--   0 nicolasagustinaguirrecampi   (501) staff       (20)      261 2023-10-18 11:32:41.000000 colorcompass-1.2.1/colorcompass.egg-info/SOURCES.txt
--rw-r--r--   0 nicolasagustinaguirrecampi   (501) staff       (20)        1 2023-10-18 11:32:41.000000 colorcompass-1.2.1/colorcompass.egg-info/dependency_links.txt
--rw-r--r--   0 nicolasagustinaguirrecampi   (501) staff       (20)       13 2023-10-18 11:32:41.000000 colorcompass-1.2.1/colorcompass.egg-info/top_level.txt
--rw-r--r--   0 nicolasagustinaguirrecampi   (501) staff       (20)       38 2023-10-18 11:32:41.596505 colorcompass-1.2.1/setup.cfg
--rw-r--r--   0 nicolasagustinaguirrecampi   (501) staff       (20)      781 2023-10-18 11:32:22.000000 colorcompass-1.2.1/setup.py
+drwxr-xr-x   0 nicolasaguirre   (501) staff       (20)        0 2024-05-22 02:01:50.322950 colorcompass-1.2.3/
+-rw-r--r--   0 nicolasaguirre   (501) staff       (20)     1077 2024-05-22 01:42:05.000000 colorcompass-1.2.3/LICENSE.md
+-rw-r--r--   0 nicolasaguirre   (501) staff       (20)     4477 2024-05-22 02:01:50.322699 colorcompass-1.2.3/PKG-INFO
+-rw-r--r--   0 nicolasaguirre   (501) staff       (20)     3251 2024-05-22 01:42:05.000000 colorcompass-1.2.3/README.md
+drwxr-xr-x   0 nicolasaguirre   (501) staff       (20)        0 2024-05-22 02:01:50.321078 colorcompass-1.2.3/colorcompass/
+-rw-r--r--   0 nicolasaguirre   (501) staff       (20)       41 2024-05-22 01:42:05.000000 colorcompass-1.2.3/colorcompass/__init__.py
+-rw-r--r--   0 nicolasaguirre   (501) staff       (20)     2628 2024-05-22 01:42:05.000000 colorcompass-1.2.3/colorcompass/color_compass.py
+-rw-r--r--   0 nicolasaguirre   (501) staff       (20)    31533 2024-05-22 01:42:05.000000 colorcompass-1.2.3/colorcompass/color_dictionary.py
+drwxr-xr-x   0 nicolasaguirre   (501) staff       (20)        0 2024-05-22 02:01:50.321776 colorcompass-1.2.3/colorcompass.egg-info/
+-rw-r--r--   0 nicolasaguirre   (501) staff       (20)     4477 2024-05-22 02:01:50.000000 colorcompass-1.2.3/colorcompass.egg-info/PKG-INFO
+-rw-r--r--   0 nicolasaguirre   (501) staff       (20)      261 2024-05-22 02:01:50.000000 colorcompass-1.2.3/colorcompass.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolasaguirre   (501) staff       (20)        1 2024-05-22 02:01:50.000000 colorcompass-1.2.3/colorcompass.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolasaguirre   (501) staff       (20)       13 2024-05-22 02:01:50.000000 colorcompass-1.2.3/colorcompass.egg-info/top_level.txt
+-rw-r--r--   0 nicolasaguirre   (501) staff       (20)       38 2024-05-22 02:01:50.323084 colorcompass-1.2.3/setup.cfg
+-rw-r--r--   0 nicolasaguirre   (501) staff       (20)     1350 2024-05-22 02:00:49.000000 colorcompass-1.2.3/setup.py
```

### Comparing `colorcompass-1.2.1/LICENSE.md` & `colorcompass-1.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `colorcompass-1.2.1/PKG-INFO` & `colorcompass-1.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,28 @@
 Metadata-Version: 2.1
 Name: colorcompass
-Version: 1.2.1
-Summary: A brief description of your project.
+Version: 1.2.3
+Summary: Converts RGB or hexadecimal values to exact color names.
 Home-page: https://github.com/NicolasAguirreCampi/ColorCompass
 Author: Nicolas Aguirre Campi
 Author-email: aguirrecampi.nicolas@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Utilities
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -85,7 +98,8 @@
 ## 📞 Contact
 
 If you have questions or issues, please [open an issue](https://github.com/NicolasAguirreCampi/ColorCompass/issues/new).
 
 ## 🙏 Acknowledgements
 
 Special thanks to [xkcd by Randall Munroe](https://blog.xkcd.com/2010/05/03/color-survey-results/) for providing an extensive collection of nearly 1000 color names and their respective codes, which was pivotal in developing this project. Although modifications were made to the original list, it served as a foundational resource in building the ColorCompass library.
+
```

### Comparing `colorcompass-1.2.1/README.md` & `colorcompass-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `colorcompass-1.2.1/colorcompass/color_compass.py` & `colorcompass-1.2.3/colorcompass/color_compass.py`

 * *Files identical despite different names*

### Comparing `colorcompass-1.2.1/colorcompass/color_dictionary.py` & `colorcompass-1.2.3/colorcompass/color_dictionary.py`

 * *Files identical despite different names*

### Comparing `colorcompass-1.2.1/colorcompass.egg-info/PKG-INFO` & `colorcompass-1.2.3/colorcompass.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,28 @@
 Metadata-Version: 2.1
 Name: colorcompass
-Version: 1.2.1
-Summary: A brief description of your project.
+Version: 1.2.3
+Summary: Converts RGB or hexadecimal values to exact color names.
 Home-page: https://github.com/NicolasAguirreCampi/ColorCompass
 Author: Nicolas Aguirre Campi
 Author-email: aguirrecampi.nicolas@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Utilities
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -85,7 +98,8 @@
 ## 📞 Contact
 
 If you have questions or issues, please [open an issue](https://github.com/NicolasAguirreCampi/ColorCompass/issues/new).
 
 ## 🙏 Acknowledgements
 
 Special thanks to [xkcd by Randall Munroe](https://blog.xkcd.com/2010/05/03/color-survey-results/) for providing an extensive collection of nearly 1000 color names and their respective codes, which was pivotal in developing this project. Although modifications were made to the original list, it served as a foundational resource in building the ColorCompass library.
+
```

