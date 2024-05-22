# Comparing `tmp/jupyterlab_language_pack_ko_kr-4.2.post0.tar.gz` & `tmp/jupyterlab_language_pack_ko_kr-4.2.post1.tar.gz`

## Comparing `jupyterlab_language_pack_ko_kr-4.2.post0.tar` & `jupyterlab_language_pack_ko_kr-4.2.post1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/.copier-answers.yml
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/CONTRIBUTORS.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/dask_labextension.po
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_archive.po
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_collaboration.po
--rw-r--r--   0        0        0     9818 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_resource_usage.po
--rw-r--r--   0        0        0   308289 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab.po
--rw-r--r--   0        0        0   150309 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_git.po
--rw-r--r--   0        0        0    64690 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_lsp.po
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_recents.po
--rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_search_replace.po
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
--rw-r--r--   0        0        0    13084 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_tour.po
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_widgets.po
--rw-r--r--   0        0        0     7470 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupytext.po
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/nbdime.po
--rw-r--r--   0        0        0    11040 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/notebook.po
--rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/retrolab.po
--rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/spellchecker.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/LICENSE.txt
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/README.md
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/pyproject.toml
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post0/PKG-INFO
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/.copier-answers.yml
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/dask_labextension.po
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_archive.po
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_collaboration.po
+-rw-r--r--   0        0        0     9818 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_resource_usage.po
+-rw-r--r--   0        0        0   308289 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab.po
+-rw-r--r--   0        0        0   150309 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_git.po
+-rw-r--r--   0        0        0    64690 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_lsp.po
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_recents.po
+-rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_search_replace.po
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
+-rw-r--r--   0        0        0    13084 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_tour.po
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_widgets.po
+-rw-r--r--   0        0        0     7470 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupytext.po
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/nbdime.po
+-rw-r--r--   0        0        0    11040 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/notebook.po
+-rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/retrolab.po
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/spellchecker.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/LICENSE.txt
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/README.md
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/pyproject.toml
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ko_kr-4.2.post1/PKG-INFO
```

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/CONTRIBUTORS.md` & `jupyterlab_language_pack_ko_kr-4.2.post1/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/dask_labextension.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/dask_labextension.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_archive.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_archive.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_collaboration.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_collaboration.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_resource_usage.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyter_resource_usage.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_git.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_git.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_lsp.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_lsp.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_recents.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_recents.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_search_replace.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_search_replace.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_tour.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_tour.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_widgets.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupyterlab_widgets.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupytext.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/jupytext.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/nbdime.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/nbdime.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/notebook.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/notebook.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/retrolab.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/retrolab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/spellchecker.po` & `jupyterlab_language_pack_ko_kr-4.2.post1/jupyterlab_language_pack_ko_KR/locale/ko_KR/LC_MESSAGES/spellchecker.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/.gitignore` & `jupyterlab_language_pack_ko_kr-4.2.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/LICENSE.txt` & `jupyterlab_language_pack_ko_kr-4.2.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/pyproject.toml` & `jupyterlab_language_pack_ko_kr-4.2.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ko_kr-4.2.post0/PKG-INFO` & `jupyterlab_language_pack_ko_kr-4.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-language-pack-ko-KR
-Version: 4.2.post0
+Version: 4.2.post1
 Summary: JupyterLab Korean (South Korea) Language Pack
 Project-URL: homepage, https://github.com/jupyterlab/language-packs
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2023 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

