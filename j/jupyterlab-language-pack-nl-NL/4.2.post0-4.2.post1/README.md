# Comparing `tmp/jupyterlab_language_pack_nl_nl-4.2.post0.tar.gz` & `tmp/jupyterlab_language_pack_nl_nl-4.2.post1.tar.gz`

## Comparing `jupyterlab_language_pack_nl_nl-4.2.post0.tar` & `jupyterlab_language_pack_nl_nl-4.2.post1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/.copier-answers.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/CONTRIBUTORS.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/dask_labextension.po
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyter_archive.po
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyter_collaboration.po
--rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyter_resource_usage.po
--rw-r--r--   0        0        0   282408 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab.po
--rw-r--r--   0        0        0   134669 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_git.po
--rw-r--r--   0        0        0    53337 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_lsp.po
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_recents.po
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_search_replace.po
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
--rw-r--r--   0        0        0    11940 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_tour.po
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_widgets.po
--rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupytext.po
--rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/nbdime.po
--rw-r--r--   0        0        0    11046 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/notebook.po
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/retrolab.po
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/spellchecker.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/LICENSE.txt
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/README.md
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/pyproject.toml
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post0/PKG-INFO
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/.copier-answers.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/dask_labextension.po
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyter_archive.po
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyter_collaboration.po
+-rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyter_resource_usage.po
+-rw-r--r--   0        0        0   282408 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab.po
+-rw-r--r--   0        0        0   134669 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_git.po
+-rw-r--r--   0        0        0    53337 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_lsp.po
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_recents.po
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_search_replace.po
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
+-rw-r--r--   0        0        0    11940 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_tour.po
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_widgets.po
+-rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupytext.po
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/nbdime.po
+-rw-r--r--   0        0        0    11046 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/notebook.po
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/retrolab.po
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/spellchecker.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/LICENSE.txt
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/README.md
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/pyproject.toml
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 jupyterlab_language_pack_nl_nl-4.2.post1/PKG-INFO
```

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/CONTRIBUTORS.md` & `jupyterlab_language_pack_nl_nl-4.2.post1/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/dask_labextension.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/dask_labextension.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyter_archive.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyter_archive.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyter_collaboration.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyter_collaboration.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyter_resource_usage.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyter_resource_usage.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_git.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_git.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_lsp.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_lsp.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_recents.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_recents.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_search_replace.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_search_replace.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_spreadsheet_editor.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_spreadsheet_editor.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_tour.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_tour.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_widgets.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupyterlab_widgets.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupytext.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/jupytext.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/nbdime.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/nbdime.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/notebook.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/notebook.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/retrolab.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/retrolab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/spellchecker.po` & `jupyterlab_language_pack_nl_nl-4.2.post1/jupyterlab_language_pack_nl_NL/locale/nl_NL/LC_MESSAGES/spellchecker.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/.gitignore` & `jupyterlab_language_pack_nl_nl-4.2.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/LICENSE.txt` & `jupyterlab_language_pack_nl_nl-4.2.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/pyproject.toml` & `jupyterlab_language_pack_nl_nl-4.2.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_nl_nl-4.2.post0/PKG-INFO` & `jupyterlab_language_pack_nl_nl-4.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-language-pack-nl-NL
-Version: 4.2.post0
+Version: 4.2.post1
 Summary: JupyterLab Dutch (Netherlands) Language Pack
 Project-URL: homepage, https://github.com/jupyterlab/language-packs
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2023 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

