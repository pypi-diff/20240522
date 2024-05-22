# Comparing `tmp/mkdocs_ai_summary-0.1.0.tar.gz` & `tmp/mkdocs_ai_summary-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_ai_summary-0.1.0.tar", last modified: Wed May 22 14:55:40 2024, max compression
+gzip compressed data, was "mkdocs_ai_summary-0.1.1.tar", last modified: Wed May 22 15:46:40 2024, max compression
```

## Comparing `mkdocs_ai_summary-0.1.0.tar` & `mkdocs_ai_summary-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yang       (501) staff       (20)        0 2024-05-22 14:55:40.244869 mkdocs_ai_summary-0.1.0/
--rw-r--r--   0 yang       (501) staff       (20)     1067 2024-05-22 14:09:36.000000 mkdocs_ai_summary-0.1.0/LICENSE
--rw-r--r--   0 yang       (501) staff       (20)     3433 2024-05-22 14:55:40.244631 mkdocs_ai_summary-0.1.0/PKG-INFO
-drwxr-xr-x   0 yang       (501) staff       (20)        0 2024-05-22 14:55:40.243056 mkdocs_ai_summary-0.1.0/mkdocs_ai_summary/
--rw-r--r--   0 yang       (501) staff       (20)        0 2024-05-22 10:47:27.000000 mkdocs_ai_summary-0.1.0/mkdocs_ai_summary/__init__.py
--rw-r--r--   0 yang       (501) staff       (20)     2706 2024-05-22 14:53:47.000000 mkdocs_ai_summary-0.1.0/mkdocs_ai_summary/plugin.py
--rw-r--r--   0 yang       (501) staff       (20)     2157 2024-05-22 14:08:04.000000 mkdocs_ai_summary-0.1.0/mkdocs_ai_summary/tongyi_api.py
-drwxr-xr-x   0 yang       (501) staff       (20)        0 2024-05-22 14:55:40.244300 mkdocs_ai_summary-0.1.0/mkdocs_ai_summary.egg-info/
--rw-r--r--   0 yang       (501) staff       (20)     3433 2024-05-22 14:55:40.000000 mkdocs_ai_summary-0.1.0/mkdocs_ai_summary.egg-info/PKG-INFO
--rw-r--r--   0 yang       (501) staff       (20)      370 2024-05-22 14:55:40.000000 mkdocs_ai_summary-0.1.0/mkdocs_ai_summary.egg-info/SOURCES.txt
--rw-r--r--   0 yang       (501) staff       (20)        1 2024-05-22 14:55:40.000000 mkdocs_ai_summary-0.1.0/mkdocs_ai_summary.egg-info/dependency_links.txt
--rw-r--r--   0 yang       (501) staff       (20)       71 2024-05-22 14:55:40.000000 mkdocs_ai_summary-0.1.0/mkdocs_ai_summary.egg-info/entry_points.txt
--rw-r--r--   0 yang       (501) staff       (20)       34 2024-05-22 14:55:40.000000 mkdocs_ai_summary-0.1.0/mkdocs_ai_summary.egg-info/requires.txt
--rw-r--r--   0 yang       (501) staff       (20)       40 2024-05-22 14:55:40.000000 mkdocs_ai_summary-0.1.0/mkdocs_ai_summary.egg-info/top_level.txt
--rw-r--r--   0 yang       (501) staff       (20)     1033 2024-05-22 14:52:49.000000 mkdocs_ai_summary-0.1.0/pyproject.toml
--rw-r--r--   0 yang       (501) staff       (20)     1397 2024-05-22 14:39:16.000000 mkdocs_ai_summary-0.1.0/readme.md
--rw-r--r--   0 yang       (501) staff       (20)       38 2024-05-22 14:55:40.244924 mkdocs_ai_summary-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:40.250344 mkdocs_ai_summary-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 15:46:30.000000 mkdocs_ai_summary-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-22 15:46:40.250344 mkdocs_ai_summary-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:40.246344 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:30.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-22 15:46:30.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-22 15:46:30.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary/tongyi_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:40.250344 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-22 15:46:40.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-22 15:46:40.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:46:40.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 15:46:40.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 15:46:40.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 15:46:40.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-22 15:46:30.000000 mkdocs_ai_summary-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-22 15:46:30.000000 mkdocs_ai_summary-0.1.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:46:40.250344 mkdocs_ai_summary-0.1.1/setup.cfg
```

### Comparing `mkdocs_ai_summary-0.1.0/LICENSE` & `mkdocs_ai_summary-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_ai_summary-0.1.0/PKG-INFO` & `mkdocs_ai_summary-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ai-summary
-Version: 0.1.0
+Version: 0.1.1
 Summary: A mkdocs plugin to generage summary with the help of AI.
 Author-email: Yang Zhang <mail@yangzhang.site>
 License: MIT License
         
         Copyright (c) 2024 Yang Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,14 +39,18 @@
 License-File: LICENSE
 Requires-Dist: mkdocs>=1.5.3
 Provides-Extra: tongyi
 Requires-Dist: dashscope; extra == "tongyi"
 
 # mkdocs-ai-summary
 
+[![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-ai-summary)](https://pypi.org/project/mkdocs-ai-summary/)
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/mkdocs-ai-summary)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-ai-summary)
+
 Generage an **ai-summary** for the page:
 ![](assets/2024-05-22-22-00-32.png)
 
 Minimal demo [aiboy996.github.io/mkdocs-ai-summary](https://aiboy996.github.io/mkdocs-ai-summary)
 
 Live demo(my homepage): [yangzhang.site](https://yangzhang.site)
```

### Comparing `mkdocs_ai_summary-0.1.0/mkdocs_ai_summary/plugin.py` & `mkdocs_ai_summary-0.1.1/mkdocs_ai_summary/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from mkdocs.config import config_options
 from mkdocs.config.defaults import MkDocsConfig
-from mkdocs.plugins import BasePlugin, get_plugin_logger
+from mkdocs.plugins import BasePlugin
 from mkdocs.structure.files import Files
 from mkdocs.structure.pages import Page
 
 import re
 import logging
 
 logger = logging.getLogger("mkdocs.plugins.ai-summary")
```

### Comparing `mkdocs_ai_summary-0.1.0/mkdocs_ai_summary/tongyi_api.py` & `mkdocs_ai_summary-0.1.1/mkdocs_ai_summary/tongyi_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -36,14 +36,15 @@
                 response.code,
                 response.message,
             )
         )
 
 
 def get_summary_tongyi(page, prompt, markdown, cache=True, cache_dir="./"):
+    question = (prompt + markdown)[: MAX_LENGTH - 10]
     if cache:
         content_md5 = md5(markdown.encode("utf-8")).hexdigest()
         cache_file = f"{cache_dir}_ai_summary_cache.json"
         if os.path.exists(cache_file):
             with open(cache_file, "r+") as f:
                 cache_dict = json.load(f)
         else:
@@ -51,23 +52,23 @@
 
         # asked before
         if page in cache_dict:
             if content_md5 == cache_dict[page]["content_md5"]:
                 ai_summary = cache_dict[page]["ai_summary"]
             # asked before, but content changed
             else:
-                ai_summary = ask(prompt + markdown)
+                ai_summary = ask(question)
         # do not aksed before
         else:
-            ai_summary = ask(prompt + markdown)
+            ai_summary = ask(question)
             cache_dict[page] = {"content_md5": content_md5, "ai_summary": ai_summary}
             with open(f"{cache_dir}/_ai_summary_cache.json", "w+") as f:
                 cache_dict = json.dump(cache_dict, f)
     else:
-        ai_summary = ask(prompt + markdown)
+        ai_summary = ask(question)
     return f"""!!! ai-summary "AI摘要 powered by [通义千问](https://tongyi.aliyun.com/)"
     {ai_summary}
 """
 
 
 if __name__ == "__main__":
     ask()
```

### Comparing `mkdocs_ai_summary-0.1.0/mkdocs_ai_summary.egg-info/PKG-INFO` & `mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ai-summary
-Version: 0.1.0
+Version: 0.1.1
 Summary: A mkdocs plugin to generage summary with the help of AI.
 Author-email: Yang Zhang <mail@yangzhang.site>
 License: MIT License
         
         Copyright (c) 2024 Yang Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,14 +39,18 @@
 License-File: LICENSE
 Requires-Dist: mkdocs>=1.5.3
 Provides-Extra: tongyi
 Requires-Dist: dashscope; extra == "tongyi"
 
 # mkdocs-ai-summary
 
+[![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-ai-summary)](https://pypi.org/project/mkdocs-ai-summary/)
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/mkdocs-ai-summary)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-ai-summary)
+
 Generage an **ai-summary** for the page:
 ![](assets/2024-05-22-22-00-32.png)
 
 Minimal demo [aiboy996.github.io/mkdocs-ai-summary](https://aiboy996.github.io/mkdocs-ai-summary)
 
 Live demo(my homepage): [yangzhang.site](https://yangzhang.site)
```

### Comparing `mkdocs_ai_summary-0.1.0/pyproject.toml` & `mkdocs_ai_summary-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["."]
 
 [project]
 name = "mkdocs-ai-summary"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.10"
 dependencies = [
     "mkdocs>=1.5.3",
 ]
 authors = [
   { name="Yang Zhang", email="mail@yangzhang.site" },
 ]
```

### Comparing `mkdocs_ai_summary-0.1.0/readme.md` & `mkdocs_ai_summary-0.1.1/readme.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # mkdocs-ai-summary
 
+[![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-ai-summary)](https://pypi.org/project/mkdocs-ai-summary/)
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/mkdocs-ai-summary)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-ai-summary)
+
 Generage an **ai-summary** for the page:
 ![](assets/2024-05-22-22-00-32.png)
 
 Minimal demo [aiboy996.github.io/mkdocs-ai-summary](https://aiboy996.github.io/mkdocs-ai-summary)
 
 Live demo(my homepage): [yangzhang.site](https://yangzhang.site)
```

