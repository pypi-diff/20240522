# Comparing `tmp/comicinfoxml-0.2.0.tar.gz` & `tmp/comicinfoxml-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comicinfoxml-0.2.0.tar", last modified: Sat Mar  9 21:53:24 2024, max compression
+gzip compressed data, was "comicinfoxml-0.2.1.tar", last modified: Wed May 22 01:35:54 2024, max compression
```

## Comparing `comicinfoxml-0.2.0.tar` & `comicinfoxml-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 21:53:24.330638 comicinfoxml-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 21:53:24.326638 comicinfoxml-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 21:53:24.326638 comicinfoxml-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-09 21:53:10.000000 comicinfoxml-0.2.0/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-09 21:53:10.000000 comicinfoxml-0.2.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-09 21:53:10.000000 comicinfoxml-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-09 21:53:10.000000 comicinfoxml-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-09 21:53:10.000000 comicinfoxml-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-09 21:53:24.330638 comicinfoxml-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-09 21:53:10.000000 comicinfoxml-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 21:53:24.330638 comicinfoxml-0.2.0/comicinfoxml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-09 21:53:24.000000 comicinfoxml-0.2.0/comicinfoxml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-09 21:53:24.000000 comicinfoxml-0.2.0/comicinfoxml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 21:53:24.000000 comicinfoxml-0.2.0/comicinfoxml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-09 21:53:24.000000 comicinfoxml-0.2.0/comicinfoxml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-09 21:53:24.000000 comicinfoxml-0.2.0/comicinfoxml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-09 21:53:24.000000 comicinfoxml-0.2.0/comicinfoxml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-03-09 21:53:10.000000 comicinfoxml-0.2.0/comicinfoxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-03-09 21:53:10.000000 comicinfoxml-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 21:53:24.330638 comicinfoxml-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:35:54.476263 comicinfoxml-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:35:54.472263 comicinfoxml-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:35:54.476263 comicinfoxml-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 01:35:46.000000 comicinfoxml-0.2.1/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-22 01:35:46.000000 comicinfoxml-0.2.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-22 01:35:46.000000 comicinfoxml-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-22 01:35:46.000000 comicinfoxml-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 01:35:46.000000 comicinfoxml-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 01:35:54.476263 comicinfoxml-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-22 01:35:46.000000 comicinfoxml-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:35:54.476263 comicinfoxml-0.2.1/comicinfoxml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 01:35:54.000000 comicinfoxml-0.2.1/comicinfoxml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-22 01:35:54.000000 comicinfoxml-0.2.1/comicinfoxml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:35:54.000000 comicinfoxml-0.2.1/comicinfoxml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 01:35:54.000000 comicinfoxml-0.2.1/comicinfoxml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 01:35:54.000000 comicinfoxml-0.2.1/comicinfoxml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 01:35:54.000000 comicinfoxml-0.2.1/comicinfoxml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14961 2024-05-22 01:35:46.000000 comicinfoxml-0.2.1/comicinfoxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-22 01:35:46.000000 comicinfoxml-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:35:54.476263 comicinfoxml-0.2.1/setup.cfg
```

### Comparing `comicinfoxml-0.2.0/.github/workflows/build.yaml` & `comicinfoxml-0.2.1/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `comicinfoxml-0.2.0/.github/workflows/release.yaml` & `comicinfoxml-0.2.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `comicinfoxml-0.2.0/.gitignore` & `comicinfoxml-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `comicinfoxml-0.2.0/LICENSE` & `comicinfoxml-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `comicinfoxml-0.2.0/PKG-INFO` & `comicinfoxml-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comicinfoxml
-Version: 0.2.0
+Version: 0.2.1
 Summary: A metadata plugin for ComicTagger implementing the ComicInfo.xml from the anansi project
 Author-email: Timmy Welch <timmy@narnian.us>
 License: MIT
 Project-URL: Homepage, https://github.com/comictagger/comicinfoxml
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `comicinfoxml-0.2.0/comicinfoxml.egg-info/PKG-INFO` & `comicinfoxml-0.2.1/comicinfoxml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comicinfoxml
-Version: 0.2.0
+Version: 0.2.1
 Summary: A metadata plugin for ComicTagger implementing the ComicInfo.xml from the anansi project
 Author-email: Timmy Welch <timmy@narnian.us>
 License: MIT
 Project-URL: Homepage, https://github.com/comictagger/comicinfoxml
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `comicinfoxml-0.2.0/comicinfoxml.py` & `comicinfoxml-0.2.1/comicinfoxml.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,37 +188,37 @@
         credit_cover_list = []
         credit_editor_list = []
         credit_translator_list = []
 
         # first, loop thru credits, and build a list for each role that CIX
         # supports
         for credit in metadata.credits:
-            if credit['role'].casefold() in GenericMetadata.writer_synonyms:
-                credit_writer_list.append(credit['person'].replace(',', ''))
+            if credit.role.casefold() in GenericMetadata.writer_synonyms:
+                credit_writer_list.append(credit.person.replace(',', ''))
 
-            if credit['role'].casefold() in GenericMetadata.penciller_synonyms:
-                credit_penciller_list.append(credit['person'].replace(',', ''))
+            if credit.role.casefold() in GenericMetadata.penciller_synonyms:
+                credit_penciller_list.append(credit.person.replace(',', ''))
 
-            if credit['role'].casefold() in GenericMetadata.inker_synonyms:
-                credit_inker_list.append(credit['person'].replace(',', ''))
+            if credit.role.casefold() in GenericMetadata.inker_synonyms:
+                credit_inker_list.append(credit.person.replace(',', ''))
 
-            if credit['role'].casefold() in GenericMetadata.colorist_synonyms:
-                credit_colorist_list.append(credit['person'].replace(',', ''))
+            if credit.role.casefold() in GenericMetadata.colorist_synonyms:
+                credit_colorist_list.append(credit.person.replace(',', ''))
 
-            if credit['role'].casefold() in GenericMetadata.letterer_synonyms:
-                credit_letterer_list.append(credit['person'].replace(',', ''))
+            if credit.role.casefold() in GenericMetadata.letterer_synonyms:
+                credit_letterer_list.append(credit.person.replace(',', ''))
 
-            if credit['role'].casefold() in GenericMetadata.cover_synonyms:
-                credit_cover_list.append(credit['person'].replace(',', ''))
+            if credit.role.casefold() in GenericMetadata.cover_synonyms:
+                credit_cover_list.append(credit.person.replace(',', ''))
 
-            if credit['role'].casefold() in GenericMetadata.editor_synonyms:
-                credit_editor_list.append(credit['person'].replace(',', ''))
+            if credit.role.casefold() in GenericMetadata.editor_synonyms:
+                credit_editor_list.append(credit.person.replace(',', ''))
 
-            if credit['role'].casefold() in GenericMetadata.translator_synonyms:
-                credit_translator_list.append(credit['person'].replace(',', ''))
+            if credit.role.casefold() in GenericMetadata.translator_synonyms:
+                credit_translator_list.append(credit.person.replace(',', ''))
 
         assign('Series', md.series)
         assign('Number', md.issue)
         assign('Count', md.issue_count)
         assign('Title', md.title)
         assign('Volume', md.volume)
         assign('Genre', md.genres)
```

### Comparing `comicinfoxml-0.2.0/pyproject.toml` & `comicinfoxml-0.2.1/pyproject.toml`

 * *Files identical despite different names*

