# Comparing `tmp/geo_roughness_tool-0.0.1.tar.gz` & `tmp/geo_roughness_tool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_roughness_tool-0.0.1.tar", last modified: Tue May 21 11:59:11 2024, max compression
+gzip compressed data, was "geo_roughness_tool-0.1.1.tar", last modified: Tue May 21 21:09:48 2024, max compression
```

## Comparing `geo_roughness_tool-0.0.1.tar` & `geo_roughness_tool-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:59:11.290348 geo_roughness_tool-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 11:59:01.000000 geo_roughness_tool-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-21 11:59:11.290348 geo_roughness_tool-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-21 11:59:01.000000 geo_roughness_tool-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:59:11.290348 geo_roughness_tool-0.0.1/geo_roughness_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-21 11:59:11.000000 geo_roughness_tool-0.0.1/geo_roughness_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 11:59:11.000000 geo_roughness_tool-0.0.1/geo_roughness_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:59:11.000000 geo_roughness_tool-0.0.1/geo_roughness_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-21 11:59:11.000000 geo_roughness_tool-0.0.1/geo_roughness_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 11:59:11.000000 geo_roughness_tool-0.0.1/geo_roughness_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:59:11.000000 geo_roughness_tool-0.0.1/geo_roughness_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:59:11.290348 geo_roughness_tool-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-21 11:59:01.000000 geo_roughness_tool-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:48.745254 geo_roughness_tool-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-21 21:09:48.745254 geo_roughness_tool-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 21:09:48.745254 geo_roughness_tool-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:48.737254 geo_roughness_tool-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:48.737254 geo_roughness_tool-0.1.1/src/geo_roughness_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:48.741254 geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/processing_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/classes/threshold_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:48.741254 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/analyze_and_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/footer_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/header_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/path_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui/preview_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:48.741254 geo_roughness_tool-0.1.1/src/geo_roughness_tool/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-21 21:09:41.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool/tests/test_application_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:09:48.741254 geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-21 21:09:48.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-21 21:09:48.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 21:09:48.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-21 21:09:48.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-21 21:09:48.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-21 21:09:48.000000 geo_roughness_tool-0.1.1/src/geo_roughness_tool.egg-info/top_level.txt
```

### Comparing `geo_roughness_tool-0.0.1/LICENSE` & `geo_roughness_tool-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.0.1/README.md` & `geo_roughness_tool-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 ## Installation Guide for GeoRoughness Tool
 
 Follow these steps to install the GeoRoughness Tool on your system. The program is available
 as a Python package and can therefore be installed on any major operating system.
 
 > [!TIP]
-> If you are not that experienced using command line tools or experience any problems during installation, please refer to the [Getting Started Wiki Page](https://github.com/lbatschelet/dem-roughness-calculator/wiki/Getting-Started) for a more detailed and OS specific installation guide.
+> If you are not that experienced using command line tools or experience any problems during installation, please refer to the [Getting Started Wiki Page](../../wiki/Getting-Started) for a more detailed and OS specific installation guide.
 
 ### Prerequisites
 
 Before you begin, ensure that your system meets the following requirements:
 - **Python 3.12 or later**: The software is built to run with Python 3.12 and above.
 - **pip**: Python's package installer, used to install the GeoRoughness Tool.
 
@@ -89,12 +89,12 @@
 > 
 > Please note that while AI has contributed to the project, it may not capture the full complexity or context of the development practices. As such, any anomalies or errors introduced by AI-generated content have been reviewed and rectified to the best of our capabilities. However, users should exercise their judgment and discretion when using or modifying this software. 
 > 
 > For any concerns or questions about the AI-generated content within this project, please feel free to contact us through the repository's issues section.
 
 ## Contributing
 
-We welcome contributions! If you have suggestions or want to report bugs, please use the [Issues](https://github.com/lbatschelet/dem-roughness-calculator/issues) section of this repository.
+We welcome contributions! If you have suggestions or want to report bugs, please use the [Issues](../../issues) section of this repository.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `geo_roughness_tool-0.0.1/setup.py` & `geo_roughness_tool-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,50 @@
+import os
 from setuptools import setup, find_packages
 
+# Read the contents of your README file
+def read(file_name):
+    with open(file_name, 'r', encoding='utf-8') as f:
+        return f.read()
+
 # Read the contents of your requirements file
-with open('requirements.txt') as f:
-    requirements = f.read().splitlines()
+def read_requirements(file_name):
+    with open(file_name, 'r', encoding='utf-8') as f:
+        return f.read().splitlines()
 
 setup(
-    name='geo_roughness_tool',
-    version='0.0.1',
-    packages=find_packages(),  # Automatically find all packages in the directory
+    name='geo-roughness-tool',
+    version='0.1.1',
+    packages=find_packages(where='src'),
+    package_dir={'': 'src'},
     url='https://github.com/lbatschelet/GeoRoughness-Tool',
-    license='GPL-3.0',
-    author='lbatschelet',
+    license='MIT',
+    author='Lukas Batschelet',
+    author_email='your-email@example.com',  # Replace with your email
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
-    install_requires=requirements,  # Install dependencies from requirements.txt
+    long_description=read('README.md'),  # Use the README.md as the long description
+    long_description_content_type='text/markdown',
+    install_requires=read_requirements('requirements.txt'),  # Install dependencies from requirements.txt
     python_requires='>=3.12',  # Specify Python version requirement
     entry_points={
         'console_scripts': [
             'georough=geo_roughness_tool.main:main',
-            'demgui=geo_roughness_tool.old_entry_points.demgui:main',
-            'demcli=geo_roughness_tool.old_entry_points.demcli:main',
+            'dingsbums=geo_roughness_tool.main:main',
+            'giraffe=geo_roughness_tool.main:main',
         ]
     },
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 4 - Beta',  # Update as appropriate for your release cycle
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.12',
         'Topic :: Scientific/Engineering :: GIS'
-    ]
+    ],
+    project_urls={  # Optional
+        'Documentation': 'https://github.com/lbatschelet/GeoRoughness-Tool/wiki',
+        'Source': 'https://github.com/lbatschelet/GeoRoughness-Tool',
+        'Tracker': 'https://github.com/lbatschelet/GeoRoughness-Tool/issues',
+    },
+    keywords='GIS, GeoTIFF, DEM, surface roughness, geographic information systems',  # Add relevant keywords
 )
```

