# Comparing `tmp/sentier_glossary-0.3.0.tar.gz` & `tmp/sentier_glossary-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentier_glossary-0.3.0.tar", last modified: Tue May 21 18:11:47 2024, max compression
+gzip compressed data, was "sentier_glossary-0.4.0.tar", last modified: Wed May 22 10:23:14 2024, max compression
```

## Comparing `sentier_glossary-0.3.0.tar` & `sentier_glossary-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:11:47.907541 sentier_glossary-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 18:11:44.000000 sentier_glossary-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:11:44.000000 sentier_glossary-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-21 18:11:47.907541 sentier_glossary-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-21 18:11:44.000000 sentier_glossary-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-21 18:11:44.000000 sentier_glossary-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:11:47.903541 sentier_glossary-0.3.0/sentier_glossary/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-21 18:11:44.000000 sentier_glossary-0.3.0/sentier_glossary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-05-21 18:11:44.000000 sentier_glossary-0.3.0/sentier_glossary/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-21 18:11:44.000000 sentier_glossary-0.3.0/sentier_glossary/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:11:47.903541 sentier_glossary-0.3.0/sentier_glossary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-21 18:11:47.000000 sentier_glossary-0.3.0/sentier_glossary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-21 18:11:47.000000 sentier_glossary-0.3.0/sentier_glossary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:11:47.000000 sentier_glossary-0.3.0/sentier_glossary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-21 18:11:47.000000 sentier_glossary-0.3.0/sentier_glossary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-21 18:11:47.000000 sentier_glossary-0.3.0/sentier_glossary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 18:11:47.907541 sentier_glossary-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:23:14.181460 sentier_glossary-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 10:23:10.000000 sentier_glossary-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:23:10.000000 sentier_glossary-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-22 10:23:14.177460 sentier_glossary-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-22 10:23:10.000000 sentier_glossary-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-22 10:23:10.000000 sentier_glossary-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:23:14.177460 sentier_glossary-0.4.0/sentier_glossary/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-22 10:23:10.000000 sentier_glossary-0.4.0/sentier_glossary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-22 10:23:10.000000 sentier_glossary-0.4.0/sentier_glossary/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-22 10:23:10.000000 sentier_glossary-0.4.0/sentier_glossary/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:23:14.177460 sentier_glossary-0.4.0/sentier_glossary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-22 10:23:14.000000 sentier_glossary-0.4.0/sentier_glossary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-22 10:23:14.000000 sentier_glossary-0.4.0/sentier_glossary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:23:14.000000 sentier_glossary-0.4.0/sentier_glossary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-22 10:23:14.000000 sentier_glossary-0.4.0/sentier_glossary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 10:23:14.000000 sentier_glossary-0.4.0/sentier_glossary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:23:14.181460 sentier_glossary-0.4.0/setup.cfg
```

### Comparing `sentier_glossary-0.3.0/LICENSE` & `sentier_glossary-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentier_glossary-0.3.0/PKG-INFO` & `sentier_glossary-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentier_glossary
-Version: 0.3.0
+Version: 0.4.0
 Summary: Client interface to sentier.dev sustainability assessment glossary
 Author-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Maintainer-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: homepage, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: tracker, https://github.com/Depart-de-Sentier/sentier_glossary/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sentier_glossary-0.3.0/README.md` & `sentier_glossary-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sentier_glossary-0.3.0/pyproject.toml` & `sentier_glossary-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sentier_glossary-0.3.0/sentier_glossary/main.py` & `sentier_glossary-0.4.0/sentier_glossary/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         Args:
             query (str): the search query string
             scope (str, CommonSchemes, None): If given, limit the search to one concept scheme
 
         Returns:
             list of resources matching the search query.
         """
-        return self._requests_get("search", {"search_term": query})["concepts"]
+        return self._requests_get("search", {"search_term": query})
 
     def semantic_search(
         self, query: str, scope: str | CommonSchemes | None = None, min_num_results: int = 10
     ) -> list[dict]:
         """Perform semantic search query.
 
         Stolen shamelessly from https://www.sbert.net/examples/applications/semantic-search/README.html#semantic-search.
```

### Comparing `sentier_glossary-0.3.0/sentier_glossary.egg-info/PKG-INFO` & `sentier_glossary-0.4.0/sentier_glossary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentier_glossary
-Version: 0.3.0
+Version: 0.4.0
 Summary: Client interface to sentier.dev sustainability assessment glossary
 Author-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Maintainer-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: homepage, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: tracker, https://github.com/Depart-de-Sentier/sentier_glossary/issues
 Classifier: Development Status :: 4 - Beta
```

