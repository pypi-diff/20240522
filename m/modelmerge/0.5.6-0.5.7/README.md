# Comparing `tmp/modelmerge-0.5.6.tar.gz` & `tmp/modelmerge-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.5.6.tar", last modified: Wed May 22 18:39:10 2024, max compression
+gzip compressed data, was "modelmerge-0.5.7.tar", last modified: Wed May 22 20:35:13 2024, max compression
```

## Comparing `modelmerge-0.5.6.tar` & `modelmerge-0.5.7.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.219945 modelmerge-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-22 18:39:01.000000 modelmerge-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-22 18:39:10.219945 modelmerge-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-22 18:39:01.000000 modelmerge-0.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:39:10.219945 modelmerge-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-22 18:39:01.000000 modelmerge-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.211945 modelmerge-0.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.211945 modelmerge-0.5.6/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.211945 modelmerge-0.5.6/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    25436 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    16024 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.215945 modelmerge-0.5.6/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/run_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.215945 modelmerge-0.5.6/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/tools/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/tools/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/tools/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.215945 modelmerge-0.5.6/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.219945 modelmerge-0.5.6/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-22 18:39:10.000000 modelmerge-0.5.6/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-22 18:39:10.000000 modelmerge-0.5.6/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:39:10.000000 modelmerge-0.5.6/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 18:39:10.000000 modelmerge-0.5.6/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 18:39:10.000000 modelmerge-0.5.6/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.219945 modelmerge-0.5.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_get_token_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_py_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:13.828406 modelmerge-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-22 20:35:04.000000 modelmerge-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-22 20:35:13.828406 modelmerge-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-22 20:35:04.000000 modelmerge-0.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:35:13.828406 modelmerge-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-22 20:35:04.000000 modelmerge-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:13.820406 modelmerge-0.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:13.820406 modelmerge-0.5.7/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:13.824406 modelmerge-0.5.7/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25436 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16024 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:13.824406 modelmerge-0.5.7/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/plugins/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/plugins/run_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:13.824406 modelmerge-0.5.7/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/tools/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/tools/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/tools/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:13.824406 modelmerge-0.5.7/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-22 20:35:04.000000 modelmerge-0.5.7/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:13.828406 modelmerge-0.5.7/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-22 20:35:13.000000 modelmerge-0.5.7/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-22 20:35:13.000000 modelmerge-0.5.7/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:35:13.000000 modelmerge-0.5.7/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 20:35:13.000000 modelmerge-0.5.7/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 20:35:13.000000 modelmerge-0.5.7/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:13.828406 modelmerge-0.5.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_get_token_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_py_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-22 20:35:04.000000 modelmerge-0.5.7/test/test_whisper.py
```

### Comparing `modelmerge-0.5.6/LICENSE` & `modelmerge-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/PKG-INFO` & `modelmerge-0.5.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.5.6
+Version: 0.5.7
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.5.6/README.md` & `modelmerge-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/src/ModelMerge/models/base.py` & `modelmerge-0.5.7/src/ModelMerge/models/base.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.5.7/src/ModelMerge/models/chatgpt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/src/ModelMerge/models/claude.py` & `modelmerge-0.5.7/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/src/ModelMerge/models/genimi.py` & `modelmerge-0.5.7/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/src/ModelMerge/models/groq.py` & `modelmerge-0.5.7/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/src/ModelMerge/plugins/config.py` & `modelmerge-0.5.7/src/ModelMerge/plugins/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/src/ModelMerge/plugins/image.py` & `modelmerge-0.5.7/src/ModelMerge/plugins/image.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.5.7/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.5.7/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/src/ModelMerge/tools/chatgpt.py` & `modelmerge-0.5.7/src/ModelMerge/tools/chatgpt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/src/ModelMerge/tools/claude.py` & `modelmerge-0.5.7/src/ModelMerge/tools/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/src/ModelMerge/tools/run.py` & `modelmerge-0.5.7/src/ModelMerge/tools/run.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/src/ModelMerge/utils/prompt.py` & `modelmerge-0.5.7/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/src/ModelMerge/utils/scripts.py` & `modelmerge-0.5.7/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.5.7/src/modelmerge.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.5.6
+Version: 0.5.7
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.5.6/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.5.7/src/modelmerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_Web_crawler.py` & `modelmerge-0.5.7/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_claude_zh_char.py` & `modelmerge-0.5.7/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_ddg_search.py` & `modelmerge-0.5.7/test/test_ddg_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_download_pdf.py` & `modelmerge-0.5.7/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_get_token_dict.py` & `modelmerge-0.5.7/test/test_get_token_dict.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_google_search.py` & `modelmerge-0.5.7/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_jieba.py` & `modelmerge-0.5.7/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_json.py` & `modelmerge-0.5.7/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_langchain_search_old.py` & `modelmerge-0.5.7/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_logging.py` & `modelmerge-0.5.7/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_ollama.py` & `modelmerge-0.5.7/test/test_ollama.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_py_run.py` & `modelmerge-0.5.7/test/test_py_run.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_requests.py` & `modelmerge-0.5.7/test/test_requests.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_tikitoken.py` & `modelmerge-0.5.7/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_token.py` & `modelmerge-0.5.7/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.6/test/test_url.py` & `modelmerge-0.5.7/test/test_url.py`

 * *Files identical despite different names*

