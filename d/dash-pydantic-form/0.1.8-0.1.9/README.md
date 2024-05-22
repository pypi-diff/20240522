# Comparing `tmp/dash_pydantic_form-0.1.8.tar.gz` & `tmp/dash_pydantic_form-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_pydantic_form-0.1.8.tar", last modified: Mon May 20 10:08:17 2024, max compression
+gzip compressed data, was "dash_pydantic_form-0.1.9.tar", last modified: Mon May 20 10:27:02 2024, max compression
```

## Comparing `dash_pydantic_form-0.1.8.tar` & `dash_pydantic_form-0.1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.421362 dash_pydantic_form-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.413362 dash_pydantic_form-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.413362 dash_pydantic_form-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.413362 dash_pydantic_form-0.1.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 10:08:17.421362 dash_pydantic_form-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.417362 dash_pydantic_form-0.1.8/dash_pydantic_form/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.417362 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/all_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/base_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/editabletable_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/markdown_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/model_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/model_list_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/form_section.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    18843 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/model_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/pydantic_form_scripts.js
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/pydantic_form_styles.css
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.421362 dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 10:08:17.000000 dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-20 10:08:17.000000 dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:08:17.000000 dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-20 10:08:17.000000 dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 10:08:17.000000 dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.417362 dash_pydantic_form-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.421362 dash_pydantic_form-0.1.8/images/
--rwxr-xr-x   0 runner    (1001) docker     (127)    47789 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/images/conditionnally-visible-field.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    55763 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/images/discriminated-union.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    15290 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/images/editable-table.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4506 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/images/form-sections.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    12406 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/images/model-list.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     8028 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/images/nested-model.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    16764 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/images/simple-form.png
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 10:08:17.421362 dash_pydantic_form-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:27:02.577296 dash_pydantic_form-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:27:02.569296 dash_pydantic_form-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:27:02.569296 dash_pydantic_form-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:27:02.569296 dash_pydantic_form-0.1.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 10:27:02.577296 dash_pydantic_form-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:27:02.573295 dash_pydantic_form-0.1.9/dash_pydantic_form/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/dash_pydantic_form/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:27:02.573295 dash_pydantic_form-0.1.9/dash_pydantic_form/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/dash_pydantic_form/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/dash_pydantic_form/fields/all_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/dash_pydantic_form/fields/base_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/dash_pydantic_form/fields/editabletable_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/dash_pydantic_form/fields/markdown_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/dash_pydantic_form/fields/model_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21497 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/dash_pydantic_form/fields/model_list_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/dash_pydantic_form/form_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/dash_pydantic_form/ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19031 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/dash_pydantic_form/model_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/dash_pydantic_form/pydantic_form_scripts.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/dash_pydantic_form/pydantic_form_styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/dash_pydantic_form/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:27:02.577296 dash_pydantic_form-0.1.9/dash_pydantic_form.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 10:27:02.000000 dash_pydantic_form-0.1.9/dash_pydantic_form.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-20 10:27:02.000000 dash_pydantic_form-0.1.9/dash_pydantic_form.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:27:02.000000 dash_pydantic_form-0.1.9/dash_pydantic_form.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-20 10:27:02.000000 dash_pydantic_form-0.1.9/dash_pydantic_form.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 10:27:02.000000 dash_pydantic_form-0.1.9/dash_pydantic_form.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:27:02.573295 dash_pydantic_form-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:27:02.577296 dash_pydantic_form-0.1.9/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47789 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/images/conditionnally-visible-field.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55763 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/images/discriminated-union.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15290 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/images/editable-table.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4506 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/images/form-sections.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12406 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/images/model-list.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8028 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/images/nested-model.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16764 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/images/simple-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 10:27:02.577296 dash_pydantic_form-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-20 10:26:51.000000 dash_pydantic_form-0.1.9/usage.py
```

### Comparing `dash_pydantic_form-0.1.8/.github/workflows/publish.yaml` & `dash_pydantic_form-0.1.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/.gitignore` & `dash_pydantic_form-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/.vscode/launch.json` & `dash_pydantic_form-0.1.9/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/CHANGELOG.md` & `dash_pydantic_form-0.1.9/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.8] - 2024-05-20
+### Added
+- ModelForm container_kwargs argument
+
 ## [0.1.7] - 2024-05-20
 ### Changed
 - Use container query to ensure the columns shrink when the form container is small
 
 ## [0.1.6] - 2024-05-20
 ### Changed
 - Always store form specs in in a `ids.form_specs_store`, not just for discriminated unions
```

### Comparing `dash_pydantic_form-0.1.8/PKG-INFO` & `dash_pydantic_form-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.8
+Version: 0.1.9
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
```

### Comparing `dash_pydantic_form-0.1.8/README.md` & `dash_pydantic_form-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form/__init__.py` & `dash_pydantic_form-0.1.9/dash_pydantic_form/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form/fields/__init__.py` & `dash_pydantic_form-0.1.9/dash_pydantic_form/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form/fields/all_fields.py` & `dash_pydantic_form-0.1.9/dash_pydantic_form/fields/all_fields.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form/fields/base_fields.py` & `dash_pydantic_form-0.1.9/dash_pydantic_form/fields/base_fields.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form/fields/editabletable_field.py` & `dash_pydantic_form-0.1.9/dash_pydantic_form/fields/editabletable_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form/fields/markdown_field.py` & `dash_pydantic_form-0.1.9/dash_pydantic_form/fields/markdown_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form/fields/model_field.py` & `dash_pydantic_form-0.1.9/dash_pydantic_form/fields/model_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form/fields/model_list_field.py` & `dash_pydantic_form-0.1.9/dash_pydantic_form/fields/model_list_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
                 ModelForm(
                     item=item,
                     aio_id=aio_id,
                     form_id=form_id,
                     path=new_parent,
                     fields_repr=fields_repr,
                     sections=sections,
+                    container_kwargs={"style": {"flex": 1}},
                 ),
             ]
             + items_deletable
             * [
                 dmc.ActionIcon(
                     DashIconify(icon="carbon:trash-can", height=16),
                     color="red",
```

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form/form_section.py` & `dash_pydantic_form-0.1.9/dash_pydantic_form/form_section.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form/ids.py` & `dash_pydantic_form-0.1.9/dash_pydantic_form/ids.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form/model_form.py` & `dash_pydantic_form-0.1.9/dash_pydantic_form/model_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,16 @@
     sections: Sections | None
         List of form sections (optional). See `Sections`.
     submit_on_enter: bool
         Whether to submit the form on enter. Default False.
         Note: this may break the behaviour of some fields (e.g. editable table), use with caution.
     excluded_fields: list[str] | None
         List of field names to exclude from the form altogether, optional.
+    container_kwargs: dict | None
+        Additional kwargs to pass to the containing div.
     """
 
     class ids:
         """Model form ids."""
 
         form = partial(form_base_id, "_pydf-form")
         main = partial(form_base_id, "_pydf-main")
@@ -98,14 +100,15 @@
         form_id: str,
         path: str = "",
         fields_repr: dict[str, Union["BaseField", dict]] | None = None,
         sections: Sections | None = None,
         submit_on_enter: bool = False,
         discriminator: str | None = None,
         excluded_fields: list[str] | None = None,
+        container_kwargs: dict | None = None,
     ) -> None:
         from dash_pydantic_form.fields import get_default_repr
 
         with contextlib.suppress(Exception):
             if issubclass(item, BaseModel):
                 item = item.model_construct()
 
@@ -212,23 +215,24 @@
                 },
                 id=self.ids.form_specs_store(aio_id, form_id, path),
             )
         )
 
         super().__init__(
             children=children,
-            style={"containerType": "inline-size"},
             **(
                 {
                     "id": self.ids.form(aio_id, form_id, path),
                     "data-entersubmits": submit_on_enter,
+                    "style": {"containerType": "inline-size"},
                 }
                 if not path
                 else {}
             ),
+            **(container_kwargs or {}),
         )
 
     @classmethod
     def grid(cls, children: Children, **kwargs):
         """Create the responsive grid for a field."""
         return dmc.SimpleGrid(children, className="pydantic-form-grid", **kwargs)
```

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form/pydantic_form_scripts.js` & `dash_pydantic_form-0.1.9/dash_pydantic_form/pydantic_form_scripts.js`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form/pydantic_form_styles.css` & `dash_pydantic_form-0.1.9/dash_pydantic_form/pydantic_form_styles.css`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form/utils.py` & `dash_pydantic_form-0.1.9/dash_pydantic_form/utils.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/PKG-INFO` & `dash_pydantic_form-0.1.9/dash_pydantic_form.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.8
+Version: 0.1.9
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
```

### Comparing `dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/SOURCES.txt` & `dash_pydantic_form-0.1.9/dash_pydantic_form.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/images/conditionnally-visible-field.gif` & `dash_pydantic_form-0.1.9/images/conditionnally-visible-field.gif`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/images/discriminated-union.gif` & `dash_pydantic_form-0.1.9/images/discriminated-union.gif`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/images/editable-table.png` & `dash_pydantic_form-0.1.9/images/editable-table.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/images/form-sections.png` & `dash_pydantic_form-0.1.9/images/form-sections.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/images/model-list.png` & `dash_pydantic_form-0.1.9/images/model-list.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/images/nested-model.png` & `dash_pydantic_form-0.1.9/images/nested-model.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/images/simple-form.png` & `dash_pydantic_form-0.1.9/images/simple-form.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/pyproject.toml` & `dash_pydantic_form-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.8/usage.py` & `dash_pydantic_form-0.1.9/usage.py`

 * *Files identical despite different names*

