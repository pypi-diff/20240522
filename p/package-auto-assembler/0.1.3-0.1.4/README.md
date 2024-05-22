# Comparing `tmp/package_auto_assembler-0.1.3.tar.gz` & `tmp/package_auto_assembler-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "package_auto_assembler-0.1.3.tar", last modified: Sat May 11 04:33:18 2024, max compression
+gzip compressed data, was "package_auto_assembler-0.1.4.tar", last modified: Wed May 22 01:11:31 2024, max compression
```

## Comparing `package_auto_assembler-0.1.3.tar` & `package_auto_assembler-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:33:18.227254 package_auto_assembler-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-11 04:28:27.000000 package_auto_assembler-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    26375 2024-05-11 04:33:18.227254 package_auto_assembler-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-11 04:28:27.000000 package_auto_assembler-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:33:18.227254 package_auto_assembler-0.1.3/package_auto_assembler/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 04:32:33.000000 package_auto_assembler-0.1.3/package_auto_assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63143 2024-05-11 04:32:33.000000 package_auto_assembler-0.1.3/package_auto_assembler/package_auto_assembler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-11 04:33:17.000000 package_auto_assembler-0.1.3/package_auto_assembler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:33:18.227254 package_auto_assembler-0.1.3/package_auto_assembler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26375 2024-05-11 04:33:18.000000 package_auto_assembler-0.1.3/package_auto_assembler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-11 04:33:18.000000 package_auto_assembler-0.1.3/package_auto_assembler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 04:33:18.000000 package_auto_assembler-0.1.3/package_auto_assembler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-11 04:33:18.000000 package_auto_assembler-0.1.3/package_auto_assembler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 04:33:18.000000 package_auto_assembler-0.1.3/package_auto_assembler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 04:33:18.227254 package_auto_assembler-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:11:31.248322 package_auto_assembler-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-22 01:07:41.000000 package_auto_assembler-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    26459 2024-05-22 01:11:31.248322 package_auto_assembler-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-22 01:07:41.000000 package_auto_assembler-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:11:31.244322 package_auto_assembler-0.1.4/package_auto_assembler/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:10:45.000000 package_auto_assembler-0.1.4/package_auto_assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64814 2024-05-22 01:10:45.000000 package_auto_assembler-0.1.4/package_auto_assembler/package_auto_assembler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-22 01:11:30.000000 package_auto_assembler-0.1.4/package_auto_assembler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:11:31.248322 package_auto_assembler-0.1.4/package_auto_assembler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26459 2024-05-22 01:11:31.000000 package_auto_assembler-0.1.4/package_auto_assembler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-22 01:11:31.000000 package_auto_assembler-0.1.4/package_auto_assembler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:11:31.000000 package_auto_assembler-0.1.4/package_auto_assembler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 01:11:31.000000 package_auto_assembler-0.1.4/package_auto_assembler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 01:11:31.000000 package_auto_assembler-0.1.4/package_auto_assembler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:11:31.248322 package_auto_assembler-0.1.4/setup.cfg
```

### Comparing `package_auto_assembler-0.1.3/LICENSE` & `package_auto_assembler-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `package_auto_assembler-0.1.3/PKG-INFO` & `package_auto_assembler-0.1.4/package_auto_assembler.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: package_auto_assembler
-Version: 0.1.3
+Name: package-auto-assembler
+Version: 0.1.4
 Summary: A tool to automate package creation within ci based on just .py and optionally .ipynb file.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','packaging']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -165,27 +165,27 @@
       <th>0</th>
       <td>2024-01-06 00:54:04</td>
       <td>example_module</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>2024-05-11 04:32:47</td>
+      <td>2024-05-22 01:10:59</td>
       <td>new_package</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>2</th>
-      <td>2024-05-11 04:32:47</td>
+      <td>2024-05-22 01:10:59</td>
       <td>new_package</td>
       <td>0.0.2</td>
     </tr>
     <tr>
       <th>3</th>
-      <td>2024-05-11 04:32:47</td>
+      <td>2024-05-22 01:10:59</td>
       <td>another_new_package</td>
       <td>0.0.1</td>
     </tr>
   </tbody>
 </table>
 </div>
 
@@ -539,44 +539,45 @@
     import attr #>=22.2.0
     import string
     import os
     import csv
     
     __design_choices__ = {}
     
-    @attr.s
-    class Shouter:
+    # Metadata for package creation
     
-        """
-        A class for managing and displaying formatted log messages.
     
-        This class uses the logging module to create and manage a logger
-        for displaying formatted messages. It provides a method to output
-        various types of lines and headers, with customizable message and
-        line lengths.
+    @attr.s
+    class ComparisonFrame:
+    
         """
+        Compares query:response pairs expected vs recieved with semantic similarity
+        and simple metrics of word count, line count etc.
     
-        # Formatting settings
-        dotline_length = attr.ib(default=50)
+        ...
     
-        # Logger settings
-        logger = attr.ib(default=None)
-        logger_name = attr.ib(default='Shouter')
-        loggerLvl = attr.ib(default=lo
+        Attributes
+        ----------
+        embedder : SentenceTransformer
+            The model used to generate embeddings for semantic comparison.
+        record_file : str
+            The name of the CSV file where queries and expected results are stored.
+        results_file : str
+            The name of the CSV file where comparison results 
 
 
 
 ```python
 ldh.dependencies_names_list
 ```
 
 
 
 
-    ['example_local_dependacy_2', 'example_local_dependacy_1']
+    ['example_local_dependacy_1', 'example_local_dependacy_2']
 
 
 
 #### Save combined module
 
 
 ```python
@@ -897,15 +898,15 @@
     setup_directory = "./example_module"
 )
 ```
 
 
 
 
-    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\ncreating example_module.egg-info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\ncreating dist\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncreating build\ncreating build/lib\ncreating build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/example_module.py -> build/lib/example_module\ninstalling to build/bdist.linux-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.linux-x86_64\ncreating build/bdist.linux-x86_64/wheel\ncreating build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.linux-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.linux-x86_64/wheel/example_module-0.0.1-py3.10.egg-info\nrunning install_scripts\ncreating build/bdist.linux-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.linux-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.linux-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/opt/hostedtoolcache/Python/3.10.14/x64/lib/python3.10/site-packages/setuptools/command/install.py:34: SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.\n  warnings.warn(\n')
+    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\ncreating example_module.egg-info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\ncreating dist\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncreating build\ncreating build/lib\ncreating build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/example_module.py -> build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ninstalling to build/bdist.linux-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.linux-x86_64\ncreating build/bdist.linux-x86_64/wheel\ncreating build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.linux-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.linux-x86_64/wheel/example_module-0.0.1-py3.10.egg-info\nrunning install_scripts\ncreating build/bdist.linux-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.linux-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.linux-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/opt/hostedtoolcache/Python/3.10.14/x64/lib/python3.10/site-packages/setuptools/command/install.py:34: SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.\n  warnings.warn(\n')
 
 
 
 ### 9. Creating release notes from commit messages
 
 
 ```python
@@ -940,15 +941,16 @@
 ```
 
 
 
 
     ['Update README',
      'Update requirements',
-     '[package_auto_assembler] improved ReleaseNotesHandler with resistance to duplicate history',
+     '[package_auto_assembler] test_install_package() method for local testing',
+     'simpler test_install_package.py script',
      'Update package version tracking files',
      'Update README',
      'Update requirements']
 
 
 
 
@@ -982,15 +984,15 @@
 ```
 
     Example filtered_messaged:
     ['[example_module] usage example for initial release notes; bugfixes for RNH', '[example_module] initial release notes handler']
     Example processed_messages:
     ['usage example for initial release notes', 'bugfixes for RNH', 'initial release notes handler']
     Example processed_note_entries:
-    ['# Release notes\n', '\n', '### 0.0.2\n', '\n', '    - usage example for initial release notes\n', '    - bugfixes for RNH\n', '    - initial release notes handler\n', '\n', '### 0.0.1\n', '    - initial version of example_module\n']
+    ['# Release notes\n', '\n', '### 0.0.2\n', '\n', '    - usage example for initial release notes\n', '\n', '    - bugfixes for RNH\n', '\n', '    - initial release notes handler\n', '\n', '### 0.0.1\n', '\n', '    - initial version of example_module\n']
 
 
 ##### - saving updated relese notes
 
 
 ```python
 rnh.existing_contents
@@ -1021,14 +1023,17 @@
 
 
     ['# Release notes\n',
      '\n',
      '### 0.0.2\n',
      '\n',
      '    - usage example for initial release notes\n',
+     '\n',
      '    - bugfixes for RNH\n',
+     '\n',
      '    - initial release notes handler\n',
      '\n',
      '### 0.0.1\n',
+     '\n',
      '    - initial version of example_module\n']
```

### Comparing `package_auto_assembler-0.1.3/README.md` & `package_auto_assembler-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,62 +14,62 @@
 - contains __package_metadata__ (won't package without it)
 - falls under common license
 
 The ones that were not packages, could still be used as packages with [this instruction](https://github.com/Kiril-Mordan/reusables/blob/main/docs/module_from_raw_file.md).
 
 ## Content:
  
-[module](python_modules/shouterlog.py) | [usage](docs/shouterlog.md) | [![PyPiVersion](https://img.shields.io/pypi/v/shouterlog)](https://pypi.org/project/shouterlog/) - Shouter Log
-
-This class uses the logging module to create and manage a logger for displaying formatted messages.
-It provides a method to output various types of lines and headers, with customizable message and line lengths.
-The purpose is to be integrated into other classes that also use logger.
-
-[module](python_modules/gridlooper.py) | [usage](docs/gridlooper.md) | [drawio: -flow](docs/gridlooper-flow.png) | [![PyPiVersion](https://img.shields.io/pypi/v/gridlooper)](https://pypi.org/project/gridlooper/) - Grid Looper
+[module](python_modules/google_drive_support.py) - Google Drive API Utilities Module
 
-A tool to run experiments based on defined grid and function with single iteration.
+This module provides a set of functions for interacting with the Google Drive API.
+It allows you to authenticate with the API, upload, download, and manage files and folders in Google Drive.
 
 [module](python_modules/package_auto_assembler.py) | [usage](docs/package_auto_assembler.md) | [drawio: -flow](docs/package_auto_assembler-flow.png) | [drawio: -usage](docs/package_auto_assembler-usage.png) | [release notes](release_notes/package_auto_assembler.md) | [![PyPiVersion](https://img.shields.io/pypi/v/package-auto-assembler)](https://pypi.org/project/package-auto-assembler/) - Package Auto Assembler
 
 This tool is meant to streamline creation of single module packages.
 Its purpose is to automate as many aspects of python package creation as possible,
 to shorten a development cycle of reusable components, maintain certain standard of quality
 for reusable code. It provides tool to simplify the process of package creatrion
 to a point that it can be triggered automatically within ci/cd pipelines,
 with minimal preparations and requirements for new modules.
 
-[module](python_modules/retriever_tunner.py) | [usage](docs/retriever_tunner.md) - Retriever tunner
-
-A simple tool to compare and tune retriever performance, given a desired ranking to strive for.
-The goal is to provide a simple metric to measure how a given retriver is close to the 'ideal', generated for example
-with a use of more expensive, slower or simply no-existant method.
-
-[module](python_modules/google_drive_support.py) - Google Drive API Utilities Module
-
-This module provides a set of functions for interacting with the Google Drive API.
-It allows you to authenticate with the API, upload, download, and manage files and folders in Google Drive.
-
 [module](python_modules/parameterframe.py) | [usage](docs/parameterframe.md) | [drawio: -flow](docs/parameterframe-flow.png) | [drawio: -schema](docs/parameterframe-schema.png) | [drawio: -usage](docs/parameterframe-usage.png) | [release notes](release_notes/parameterframe.md) | [![PyPiVersion](https://img.shields.io/pypi/v/parameterframe)](https://pypi.org/project/parameterframe/) - Parameterframe
 
 The module provides an interface for managing solution parameters.
 It allows for the structured storage and retrieval of parameter sets from a database.
 
 [module](python_modules/comparisonframe.py) | [usage](docs/comparisonframe.md) | [plantuml](docs/comparisonframe_plantuml.png) - Comparison Frame
 
 Designed to automate and streamline the process of comparing textual data, particularly focusing on various metrics
 such as character and word count, punctuation usage, and semantic similarity.
 It's particularly useful for scenarios where consistent text analysis is required,
 such as evaluating the performance of natural language processing models, monitoring content quality,
 or tracking changes in textual data over time using manual evaluation.
 
+[module](python_modules/shouterlog.py) | [usage](docs/shouterlog.md) | [![PyPiVersion](https://img.shields.io/pypi/v/shouterlog)](https://pypi.org/project/shouterlog/) - Shouter Log
+
+This class uses the logging module to create and manage a logger for displaying formatted messages.
+It provides a method to output various types of lines and headers, with customizable message and line lengths.
+The purpose is to be integrated into other classes that also use logger.
+
+[module](python_modules/gridlooper.py) | [usage](docs/gridlooper.md) | [drawio: -flow](docs/gridlooper-flow.png) | [release notes](release_notes/gridlooper.md) | [![PyPiVersion](https://img.shields.io/pypi/v/gridlooper)](https://pypi.org/project/gridlooper/) - Grid Looper
+
+A tool to run experiments based on defined grid and function with single iteration.
+
 [module](python_modules/mocker_db.py) | [usage](docs/mocker_db.md) | [drawio: -flow](docs/mocker_db-flow.png) | [release notes](release_notes/mocker_db.md) | [![PyPiVersion](https://img.shields.io/pypi/v/mocker-db)](https://pypi.org/project/mocker-db/) - MockerDB
 
 A python module that contains mock vector database like solution built around
 dictionary data type. It contains methods necessary to interact with this 'database',
 embed, search and persist.
 
 [module](python_modules/search_based_extractor.py) | [usage](docs/search_based_extractor.md) - Search Based Extractor
 
 Utility to simplify webscraping by taking advantave of search and assumptions about html structure.
 Extractor allows to find parent html element that contains searched term, record path to it in a file
 and reuse that to scrape data with same html structure.
 
+[module](python_modules/retriever_tunner.py) | [usage](docs/retriever_tunner.md) - Retriever tunner
+
+A simple tool to compare and tune retriever performance, given a desired ranking to strive for.
+The goal is to provide a simple metric to measure how a given retriver is close to the 'ideal', generated for example
+with a use of more expensive, slower or simply no-existant method.
+
```

### Comparing `package_auto_assembler-0.1.3/package_auto_assembler/package_auto_assembler.py` & `package_auto_assembler-0.1.4/package_auto_assembler/package_auto_assembler.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 to a point that it can be triggered automatically within ci/cd pipelines,
 with minimal preparations and requirements for new modules.
 """
 
 # Imports
 import logging
 import os
+import sys
 import ast
 import json
 import csv
 import codecs
 from datetime import datetime
 import re
 import subprocess
@@ -1316,45 +1317,45 @@
 
             self.logger = logger
 
     def _deduplicate_with_exceptions(self,
                                      lst : list):
 
         seen = set()
-        buffer = []
         deduplicated = []
-        version_headers = []
+        version_headers = set()
 
-        for item in lst:
-
-            # start filling buffor after version is detected
+        # Reverse iteration
+        for item in reversed(lst):
+            # If it's a version header, handle it differently
             if item.startswith("###"):
-
-                if item in version_headers:
-                    seen.add(item)
-                else:
-                    deduplicated += buffer
-
-                    if deduplicated[-1] != "\n":
+                if item not in version_headers:
+                    version_headers.add(item)
+                    if deduplicated and deduplicated[-1] != "\n":
                         deduplicated.append("\n")
-
-                    version_headers.append(item)
-                if deduplicated[-1] != "\n":
-                    buffer.append("\n")
-
-            if item != lst[-1]:
-                # clean buffor when version is detected
-                if item.startswith("###"):
-                    buffer = []
+                    deduplicated.append(item)
+                    deduplicated.append("\n")  # Ensure newline after version header
             else:
-                # in the end append buffor to deduplicated
-                buffer.append(item)
-                deduplicated += buffer
-
-            buffer.append(item)
+                if item not in seen:
+                    if item == "\n" and (not deduplicated or deduplicated[-1] == "\n"):
+                        # Skip consecutive newlines
+                        continue
+                    seen.add(item)
+                    deduplicated.append(item)
+                    if item != "\n" and (deduplicated and deduplicated[-1] != "\n"):
+                        deduplicated.append("\n")  # Ensure newline after each item
+
+        # Reverse the result to restore original order
+        deduplicated.reverse()
+
+        # Clean up leading and trailing newlines
+        while deduplicated and deduplicated[0] == "\n":
+            deduplicated.pop(0)
+        while deduplicated and deduplicated[-1] == "\n":
+            deduplicated.pop()
 
         return deduplicated
 
     def _get_commits_since_last_merge(self, n_last_messages : int = 1):
 
         # First, find the last merge commit
         find_merge_command = ["git", "log", "--merges", "--format=%H", "-n", str(n_last_messages)]
@@ -1778,26 +1779,30 @@
         )
 
         # switch filepath for the combined one
         self.module_filepath = save_filepath
 
     def add_requirements_from_module(self,
                                      module_filepath : str = None,
-                                     import_mappings : str = None):
+                                     import_mappings : str = None,
+                                     check_vulnerabilities : bool = None):
 
         """
         Extract and add requirements from the module.
         """
 
         if self.requirements_h is None:
             self._initialize_requirements_handler()
 
         if module_filepath is None:
             module_filepath = self.module_filepath
 
+        if check_vulnerabilities is None:
+            check_vulnerabilities = self.check_vulnerabilities
+
         if import_mappings is None:
 
             if self.mapping_filepath is None:
                 import_mappings = {}
             else:
                 import_mappings = self.import_mapping_h.load_package_mappings()
 
@@ -1805,15 +1810,16 @@
 
         # extracting package requirements
         self.requirements_list = self.requirements_list + \
             self.requirements_h.extract_requirements(
                 package_mappings=import_mappings,
                 module_filepath=module_filepath,
                 custom_modules=custom_modules)
-        self.requirements_h.check_vulnerabilities()
+        if check_vulnerabilities:
+            self.requirements_h.check_vulnerabilities()
 
     def add_readme(self,
                     example_notebook_path : str = None,
                     output_path : str = None,
                     execute_notebook : bool = None):
 
         """
@@ -1884,7 +1890,31 @@
         # Define the command as a list of arguments
         command = ["python", os.path.join(setup_directory, "setup.py"), "sdist", "bdist_wheel"]
 
         # Execute the command
         result = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
 
         return result
+
+    def test_install_package(self,
+                             module_name : str = None,
+                             remove_temp_files : bool = True):
+
+        """
+        Test install package to environment and optional remove temp files.
+        """
+
+        if module_name is None:
+            module_name = self.module_name
+
+        # Reinstall the module from the wheel file
+        wheel_files = [f for f in os.listdir('dist') if f.endswith('-py3-none-any.whl')]
+        for wheel_file in wheel_files:
+            subprocess.run([sys.executable, "-m", "pip", "install", "--force-reinstall",
+                            os.path.join('dist', wheel_file)], check=True)
+
+        if remove_temp_files:
+            # Clean up the build directories and other generated files
+            shutil.rmtree('build', ignore_errors=True)
+            shutil.rmtree('dist', ignore_errors=True)
+            shutil.rmtree(module_name, ignore_errors=True)
+            shutil.rmtree(f"{module_name}.egg-info", ignore_errors=True)
```

### Comparing `package_auto_assembler-0.1.3/package_auto_assembler/setup.py` & `package_auto_assembler-0.1.4/package_auto_assembler/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="package_auto_assembler",
     packages=["package_auto_assembler"],
-    install_requires=['### package_auto_assembler.py', 'nbconvert', 'attrs>=22.2.0', 'nbformat', 'pyyaml', 'pandas', 'stdlib-list', 'pip_audit==2.7.3'],
+    install_requires=['### package_auto_assembler.py', 'pandas', 'pip_audit==2.7.3', 'nbformat', 'pyyaml', 'attrs>=22.2.0', 'stdlib-list', 'nbconvert'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to automate package creation within ci based on just .py and optionally .ipynb file.", keywords="['python', 'packaging']", version="0.1.3"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to automate package creation within ci based on just .py and optionally .ipynb file.", keywords="['python', 'packaging']", version="0.1.4"
 )
```

### Comparing `package_auto_assembler-0.1.3/package_auto_assembler.egg-info/PKG-INFO` & `package_auto_assembler-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: package-auto-assembler
-Version: 0.1.3
+Name: package_auto_assembler
+Version: 0.1.4
 Summary: A tool to automate package creation within ci based on just .py and optionally .ipynb file.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','packaging']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -165,27 +165,27 @@
       <th>0</th>
       <td>2024-01-06 00:54:04</td>
       <td>example_module</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>2024-05-11 04:32:47</td>
+      <td>2024-05-22 01:10:59</td>
       <td>new_package</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>2</th>
-      <td>2024-05-11 04:32:47</td>
+      <td>2024-05-22 01:10:59</td>
       <td>new_package</td>
       <td>0.0.2</td>
     </tr>
     <tr>
       <th>3</th>
-      <td>2024-05-11 04:32:47</td>
+      <td>2024-05-22 01:10:59</td>
       <td>another_new_package</td>
       <td>0.0.1</td>
     </tr>
   </tbody>
 </table>
 </div>
 
@@ -539,44 +539,45 @@
     import attr #>=22.2.0
     import string
     import os
     import csv
     
     __design_choices__ = {}
     
-    @attr.s
-    class Shouter:
+    # Metadata for package creation
     
-        """
-        A class for managing and displaying formatted log messages.
     
-        This class uses the logging module to create and manage a logger
-        for displaying formatted messages. It provides a method to output
-        various types of lines and headers, with customizable message and
-        line lengths.
+    @attr.s
+    class ComparisonFrame:
+    
         """
+        Compares query:response pairs expected vs recieved with semantic similarity
+        and simple metrics of word count, line count etc.
     
-        # Formatting settings
-        dotline_length = attr.ib(default=50)
+        ...
     
-        # Logger settings
-        logger = attr.ib(default=None)
-        logger_name = attr.ib(default='Shouter')
-        loggerLvl = attr.ib(default=lo
+        Attributes
+        ----------
+        embedder : SentenceTransformer
+            The model used to generate embeddings for semantic comparison.
+        record_file : str
+            The name of the CSV file where queries and expected results are stored.
+        results_file : str
+            The name of the CSV file where comparison results 
 
 
 
 ```python
 ldh.dependencies_names_list
 ```
 
 
 
 
-    ['example_local_dependacy_2', 'example_local_dependacy_1']
+    ['example_local_dependacy_1', 'example_local_dependacy_2']
 
 
 
 #### Save combined module
 
 
 ```python
@@ -897,15 +898,15 @@
     setup_directory = "./example_module"
 )
 ```
 
 
 
 
-    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\ncreating example_module.egg-info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\ncreating dist\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncreating build\ncreating build/lib\ncreating build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/example_module.py -> build/lib/example_module\ninstalling to build/bdist.linux-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.linux-x86_64\ncreating build/bdist.linux-x86_64/wheel\ncreating build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.linux-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.linux-x86_64/wheel/example_module-0.0.1-py3.10.egg-info\nrunning install_scripts\ncreating build/bdist.linux-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.linux-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.linux-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/opt/hostedtoolcache/Python/3.10.14/x64/lib/python3.10/site-packages/setuptools/command/install.py:34: SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.\n  warnings.warn(\n')
+    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\ncreating example_module.egg-info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\ncreating dist\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncreating build\ncreating build/lib\ncreating build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/example_module.py -> build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ninstalling to build/bdist.linux-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.linux-x86_64\ncreating build/bdist.linux-x86_64/wheel\ncreating build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.linux-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.linux-x86_64/wheel/example_module-0.0.1-py3.10.egg-info\nrunning install_scripts\ncreating build/bdist.linux-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.linux-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.linux-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/opt/hostedtoolcache/Python/3.10.14/x64/lib/python3.10/site-packages/setuptools/command/install.py:34: SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.\n  warnings.warn(\n')
 
 
 
 ### 9. Creating release notes from commit messages
 
 
 ```python
@@ -940,15 +941,16 @@
 ```
 
 
 
 
     ['Update README',
      'Update requirements',
-     '[package_auto_assembler] improved ReleaseNotesHandler with resistance to duplicate history',
+     '[package_auto_assembler] test_install_package() method for local testing',
+     'simpler test_install_package.py script',
      'Update package version tracking files',
      'Update README',
      'Update requirements']
 
 
 
 
@@ -982,15 +984,15 @@
 ```
 
     Example filtered_messaged:
     ['[example_module] usage example for initial release notes; bugfixes for RNH', '[example_module] initial release notes handler']
     Example processed_messages:
     ['usage example for initial release notes', 'bugfixes for RNH', 'initial release notes handler']
     Example processed_note_entries:
-    ['# Release notes\n', '\n', '### 0.0.2\n', '\n', '    - usage example for initial release notes\n', '    - bugfixes for RNH\n', '    - initial release notes handler\n', '\n', '### 0.0.1\n', '    - initial version of example_module\n']
+    ['# Release notes\n', '\n', '### 0.0.2\n', '\n', '    - usage example for initial release notes\n', '\n', '    - bugfixes for RNH\n', '\n', '    - initial release notes handler\n', '\n', '### 0.0.1\n', '\n', '    - initial version of example_module\n']
 
 
 ##### - saving updated relese notes
 
 
 ```python
 rnh.existing_contents
@@ -1021,14 +1023,17 @@
 
 
     ['# Release notes\n',
      '\n',
      '### 0.0.2\n',
      '\n',
      '    - usage example for initial release notes\n',
+     '\n',
      '    - bugfixes for RNH\n',
+     '\n',
      '    - initial release notes handler\n',
      '\n',
      '### 0.0.1\n',
+     '\n',
      '    - initial version of example_module\n']
```

