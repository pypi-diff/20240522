# Comparing `tmp/rsdb_utils-0.1.post1.tar.gz` & `tmp/rsdb_utils-0.1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsdb_utils-0.1.post1.tar", last modified: Wed May 22 12:14:17 2024, max compression
+gzip compressed data, was "rsdb_utils-0.1.post2.tar", last modified: Wed May 22 12:25:36 2024, max compression
```

## Comparing `rsdb_utils-0.1.post1.tar` & `rsdb_utils-0.1.post2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:14:17.061647 rsdb_utils-0.1.post1/
--rw-rw-r--   0 romain    (1000) romain    (1000)    35149 2023-06-19 14:21:45.000000 rsdb_utils-0.1.post1/LICENCE.txt
--rw-r--r--   0 romain    (1000) romain    (1000)    45540 2024-05-22 12:14:17.061647 rsdb_utils-0.1.post1/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)     3938 2024-05-22 12:12:03.000000 rsdb_utils-0.1.post1/README.md
--rw-rw-r--   0 romain    (1000) romain    (1000)     1221 2024-05-22 12:12:58.000000 rsdb_utils-0.1.post1/pyproject.toml
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:14:17.061647 rsdb_utils-0.1.post1/rsdb_utils/
--rw-rw-r--   0 romain    (1000) romain    (1000)      279 2024-05-22 11:43:31.000000 rsdb_utils-0.1.post1/rsdb_utils/__init__.py
--rw-rw-r--   0 romain    (1000) romain    (1000)     7383 2024-05-22 11:43:12.000000 rsdb_utils-0.1.post1/rsdb_utils/utils.py
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:14:17.061647 rsdb_utils-0.1.post1/rsdb_utils.egg-info/
--rw-r--r--   0 romain    (1000) romain    (1000)    45540 2024-05-22 12:14:17.000000 rsdb_utils-0.1.post1/rsdb_utils.egg-info/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)      263 2024-05-22 12:14:17.000000 rsdb_utils-0.1.post1/rsdb_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)        1 2024-05-22 12:14:17.000000 rsdb_utils-0.1.post1/rsdb_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       69 2024-05-22 12:14:17.000000 rsdb_utils-0.1.post1/rsdb_utils.egg-info/requires.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       11 2024-05-22 12:14:17.000000 rsdb_utils-0.1.post1/rsdb_utils.egg-info/top_level.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       38 2024-05-22 12:14:17.065647 rsdb_utils-0.1.post1/setup.cfg
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:14:17.061647 rsdb_utils-0.1.post1/tests/
--rw-rw-r--   0 romain    (1000) romain    (1000)     3230 2024-05-22 11:43:22.000000 rsdb_utils-0.1.post1/tests/tests.py
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:25:36.074630 rsdb_utils-0.1.post2/
+-rw-rw-r--   0 romain    (1000) romain    (1000)    35149 2023-06-19 14:21:45.000000 rsdb_utils-0.1.post2/LICENCE.txt
+-rw-r--r--   0 romain    (1000) romain    (1000)    45543 2024-05-22 12:25:36.070630 rsdb_utils-0.1.post2/PKG-INFO
+-rw-rw-r--   0 romain    (1000) romain    (1000)     3938 2024-05-22 12:12:03.000000 rsdb_utils-0.1.post2/README.md
+-rw-rw-r--   0 romain    (1000) romain    (1000)     1224 2024-05-22 12:25:09.000000 rsdb_utils-0.1.post2/pyproject.toml
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:25:36.070630 rsdb_utils-0.1.post2/rsdb_utils/
+-rw-rw-r--   0 romain    (1000) romain    (1000)      279 2024-05-22 11:43:31.000000 rsdb_utils-0.1.post2/rsdb_utils/__init__.py
+-rw-rw-r--   0 romain    (1000) romain    (1000)     7383 2024-05-22 11:43:12.000000 rsdb_utils-0.1.post2/rsdb_utils/utils.py
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:25:36.070630 rsdb_utils-0.1.post2/rsdb_utils.egg-info/
+-rw-r--r--   0 romain    (1000) romain    (1000)    45543 2024-05-22 12:25:36.000000 rsdb_utils-0.1.post2/rsdb_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 romain    (1000) romain    (1000)      263 2024-05-22 12:25:36.000000 rsdb_utils-0.1.post2/rsdb_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)        1 2024-05-22 12:25:36.000000 rsdb_utils-0.1.post2/rsdb_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       69 2024-05-22 12:25:36.000000 rsdb_utils-0.1.post2/rsdb_utils.egg-info/requires.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       11 2024-05-22 12:25:36.000000 rsdb_utils-0.1.post2/rsdb_utils.egg-info/top_level.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       38 2024-05-22 12:25:36.074630 rsdb_utils-0.1.post2/setup.cfg
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 12:25:36.070630 rsdb_utils-0.1.post2/tests/
+-rw-rw-r--   0 romain    (1000) romain    (1000)     3230 2024-05-22 11:43:22.000000 rsdb_utils-0.1.post2/tests/tests.py
```

### Comparing `rsdb_utils-0.1.post1/LICENCE.txt` & `rsdb_utils-0.1.post2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `rsdb_utils-0.1.post1/PKG-INFO` & `rsdb_utils-0.1.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsdb-utils
-Version: 0.1.post1
+Version: 0.1.post2
 Summary: Utils to process the Regime Shifts DataBase CSV and parquet files
 Author-email: Romain Thomas <romain.thomas@su.se>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,15 +674,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/romain894/rsdb-utils
+Project-URL: Homepage, https://github.com/regimeshifts/rsdb-utils
 Project-URL: Project website, https://www.regimeshifts.org/
 Keywords: Regime Shifts,Regime Shifts DataBase,RSDB,Ecosystems,Ecology,Social-ecological systems,Data analysis,Scientific research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
```

### Comparing `rsdb_utils-0.1.post1/README.md` & `rsdb_utils-0.1.post2/README.md`

 * *Files identical despite different names*

### Comparing `rsdb_utils-0.1.post1/pyproject.toml` & `rsdb_utils-0.1.post2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=65", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rsdb-utils"
-version = "0.1.post1"
+version = "0.1.post2"
 description = "Utils to process the Regime Shifts DataBase CSV and parquet files"
 readme = "README.md"
 authors = [{ name = "Romain Thomas", email = "romain.thomas@su.se" }]
 license = {file = "LICENCE.txt"}
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -38,9 +38,9 @@
 ]
 requires-python = ">=3.9"
 
 [tool.setuptools]
 packages = ["rsdb_utils"]
 
 [project.urls]
-Homepage = "https://github.com/romain894/rsdb-utils"
+Homepage = "https://github.com/regimeshifts/rsdb-utils"
 "Project website" = "https://www.regimeshifts.org/"
```

### Comparing `rsdb_utils-0.1.post1/rsdb_utils/utils.py` & `rsdb_utils-0.1.post2/rsdb_utils/utils.py`

 * *Files identical despite different names*

### Comparing `rsdb_utils-0.1.post1/rsdb_utils.egg-info/PKG-INFO` & `rsdb_utils-0.1.post2/rsdb_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsdb-utils
-Version: 0.1.post1
+Version: 0.1.post2
 Summary: Utils to process the Regime Shifts DataBase CSV and parquet files
 Author-email: Romain Thomas <romain.thomas@su.se>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,15 +674,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/romain894/rsdb-utils
+Project-URL: Homepage, https://github.com/regimeshifts/rsdb-utils
 Project-URL: Project website, https://www.regimeshifts.org/
 Keywords: Regime Shifts,Regime Shifts DataBase,RSDB,Ecosystems,Ecology,Social-ecological systems,Data analysis,Scientific research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
```

### Comparing `rsdb_utils-0.1.post1/tests/tests.py` & `rsdb_utils-0.1.post2/tests/tests.py`

 * *Files identical despite different names*

