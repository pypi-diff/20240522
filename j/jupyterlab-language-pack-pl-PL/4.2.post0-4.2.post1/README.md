# Comparing `tmp/jupyterlab_language_pack_pl_pl-4.2.post0.tar.gz` & `tmp/jupyterlab_language_pack_pl_pl-4.2.post1.tar.gz`

## Comparing `jupyterlab_language_pack_pl_pl-4.2.post0.tar` & `jupyterlab_language_pack_pl_pl-4.2.post1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/.copier-answers.yml
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/CONTRIBUTORS.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/dask_labextension.po
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyter_archive.po
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyter_collaboration.po
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyter_resource_usage.po
--rw-r--r--   0        0        0   298667 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab.po
--rw-r--r--   0        0        0   144778 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_git.po
--rw-r--r--   0        0        0    61011 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_lsp.po
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_recents.po
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_search_replace.po
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
--rw-r--r--   0        0        0    13106 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_tour.po
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_widgets.po
--rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupytext.po
--rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/nbdime.po
--rw-r--r--   0        0        0    11193 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/notebook.po
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/retrolab.po
--rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/spellchecker.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/LICENSE.txt
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/README.md
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/pyproject.toml
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post0/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/.copier-answers.yml
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/dask_labextension.po
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyter_archive.po
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyter_collaboration.po
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyter_resource_usage.po
+-rw-r--r--   0        0        0   298667 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab.po
+-rw-r--r--   0        0        0   144778 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_git.po
+-rw-r--r--   0        0        0    61011 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_lsp.po
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_recents.po
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_search_replace.po
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
+-rw-r--r--   0        0        0    13106 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_tour.po
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_widgets.po
+-rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupytext.po
+-rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/nbdime.po
+-rw-r--r--   0        0        0    11193 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/notebook.po
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/retrolab.po
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/spellchecker.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/LICENSE.txt
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/README.md
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/pyproject.toml
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pl_pl-4.2.post1/PKG-INFO
```

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/CONTRIBUTORS.md` & `jupyterlab_language_pack_pl_pl-4.2.post1/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/dask_labextension.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/dask_labextension.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyter_archive.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyter_archive.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyter_collaboration.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyter_collaboration.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyter_resource_usage.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyter_resource_usage.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_git.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_git.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_lsp.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_lsp.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_recents.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_recents.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_search_replace.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_search_replace.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_spreadsheet_editor.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_spreadsheet_editor.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_tour.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_tour.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_widgets.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupyterlab_widgets.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupytext.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/jupytext.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/nbdime.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/nbdime.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/notebook.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/notebook.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/retrolab.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/retrolab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/spellchecker.po` & `jupyterlab_language_pack_pl_pl-4.2.post1/jupyterlab_language_pack_pl_PL/locale/pl_PL/LC_MESSAGES/spellchecker.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/.gitignore` & `jupyterlab_language_pack_pl_pl-4.2.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/LICENSE.txt` & `jupyterlab_language_pack_pl_pl-4.2.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/pyproject.toml` & `jupyterlab_language_pack_pl_pl-4.2.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pl_pl-4.2.post0/PKG-INFO` & `jupyterlab_language_pack_pl_pl-4.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-language-pack-pl-PL
-Version: 4.2.post0
+Version: 4.2.post1
 Summary: JupyterLab Polish (Poland) Language Pack
 Project-URL: homepage, https://github.com/jupyterlab/language-packs
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2023 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

