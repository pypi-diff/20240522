# Comparing `tmp/modelmerge-0.5.5.tar.gz` & `tmp/modelmerge-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.5.5.tar", last modified: Tue May 21 07:05:39 2024, max compression
+gzip compressed data, was "modelmerge-0.5.6.tar", last modified: Wed May 22 18:39:10 2024, max compression
```

## Comparing `modelmerge-0.5.5.tar` & `modelmerge-0.5.6.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.339171 modelmerge-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-21 07:05:30.000000 modelmerge-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-21 07:05:39.339171 modelmerge-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-21 07:05:30.000000 modelmerge-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 07:05:39.339171 modelmerge-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-21 07:05:30.000000 modelmerge-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.331171 modelmerge-0.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.331171 modelmerge-0.5.5/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.331171 modelmerge-0.5.5/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26007 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    16005 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.331171 modelmerge-0.5.5/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/plugins/run_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.335171 modelmerge-0.5.5/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/tools/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/tools/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/tools/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.335171 modelmerge-0.5.5/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-21 07:05:30.000000 modelmerge-0.5.5/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.339171 modelmerge-0.5.5/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-21 07:05:39.000000 modelmerge-0.5.5/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-21 07:05:39.000000 modelmerge-0.5.5/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:05:39.000000 modelmerge-0.5.5/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-21 07:05:39.000000 modelmerge-0.5.5/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 07:05:39.000000 modelmerge-0.5.5/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:05:39.339171 modelmerge-0.5.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_get_token_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_py_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-21 07:05:30.000000 modelmerge-0.5.5/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.219945 modelmerge-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-22 18:39:01.000000 modelmerge-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-22 18:39:10.219945 modelmerge-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-22 18:39:01.000000 modelmerge-0.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:39:10.219945 modelmerge-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-22 18:39:01.000000 modelmerge-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.211945 modelmerge-0.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.211945 modelmerge-0.5.6/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.211945 modelmerge-0.5.6/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25436 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16024 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.215945 modelmerge-0.5.6/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/run_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.215945 modelmerge-0.5.6/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/tools/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/tools/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/tools/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.215945 modelmerge-0.5.6/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-22 18:39:01.000000 modelmerge-0.5.6/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.219945 modelmerge-0.5.6/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-22 18:39:10.000000 modelmerge-0.5.6/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-22 18:39:10.000000 modelmerge-0.5.6/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:39:10.000000 modelmerge-0.5.6/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 18:39:10.000000 modelmerge-0.5.6/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 18:39:10.000000 modelmerge-0.5.6/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:39:10.219945 modelmerge-0.5.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_get_token_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_py_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-22 18:39:01.000000 modelmerge-0.5.6/test/test_whisper.py
```

### Comparing `modelmerge-0.5.5/LICENSE` & `modelmerge-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/PKG-INFO` & `modelmerge-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.5.5
+Version: 0.5.6
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.5.5/README.md` & `modelmerge-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.5.6/src/ModelMerge/models/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from pathlib import Path
 from typing import AsyncGenerator, Set
 
 import httpx
 import requests
 import tiktoken
 
-from .config import BaseLLM, PLUGINS
+from .base import BaseLLM
+from ..plugins import PLUGINS
 from ..utils.scripts import check_json
 from ..tools import get_tools_result, function_call_list
 
 def get_filtered_keys_from_object(obj: object, *keys: str) -> Set[str]:
     """
     Get filtered list of object variable names.
     :param keys: List of keys to include. If the first key is "not", the remaining keys will be removed from the class keys.
@@ -288,15 +289,14 @@
         }
         json_post_body.update(copy.deepcopy(body))
         if all(value == False for value in PLUGINS.values()) or self.use_plugins == False:
             return json_post_body
         json_post_body.update(copy.deepcopy(function_call_list["base"]))
         for item in PLUGINS.keys():
             try:
-                # print(item, PLUGINS[item])
                 if PLUGINS[item]:
                     json_post_body["functions"].append(function_call_list[item])
             except:
                 pass
 
         return json_post_body
 
@@ -548,37 +548,14 @@
             role=role,
             convo_id=convo_id,
             **kwargs,
         )
         full_response: str = "".join([r async for r in response])
         return full_response
 
-    def ask(
-        self,
-        prompt: str,
-        role: str = "user",
-        convo_id: str = "default",
-        model: str = None,
-        pass_history: bool = True,
-        **kwargs,
-    ) -> str:
-        """
-        Non-streaming ask
-        """
-        response = self.ask_stream(
-            prompt=prompt,
-            role=role,
-            convo_id=convo_id,
-            model=model,
-            pass_history=pass_history,
-            **kwargs,
-        )
-        full_response: str = "".join(response)
-        return full_response
-
     def rollback(self, n: int = 1, convo_id: str = "default") -> None:
         """
         Rollback the conversation
         """
         for _ in range(n):
             self.conversation[convo_id].pop()
```

### Comparing `modelmerge-0.5.5/src/ModelMerge/models/claude.py` & `modelmerge-0.5.6/src/ModelMerge/models/claude.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import json
 import copy
 import tiktoken
 import requests
 
-from .config import BaseLLM, PLUGINS
+from .base import BaseLLM
+from ..plugins import PLUGINS
 from ..utils.scripts import check_json
 from ..tools import get_tools_result, claude_tools_list
 
 class claudeConversation(dict):
     def Conversation(self, index):
         conversation_list = super().__getitem__(index)
         return "\n\n" + "\n\n".join([f"{item['role']}:{item['content']}" for item in conversation_list]) + "\n\nAssistant:"
```

### Comparing `modelmerge-0.5.5/src/ModelMerge/models/genimi.py` & `modelmerge-0.5.6/src/ModelMerge/models/genimi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import json
 import requests
 import tiktoken
 
-from .config import BaseLLM
+from .base import BaseLLM
 
 class gemini(BaseLLM):
     def __init__(
         self,
         api_key: str,
         engine: str = os.environ.get("GPT_ENGINE") or "gemini-1.5-pro-latest",
         api_url: str = "https://generativelanguage.googleapis.com/v1beta/models/{model}:{stream}?key={api_key}",
```

### Comparing `modelmerge-0.5.5/src/ModelMerge/models/groq.py` & `modelmerge-0.5.6/src/ModelMerge/models/groq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import json
 import requests
 import tiktoken
 
-from .config import BaseLLM
+from .base import BaseLLM
 
 class groq(BaseLLM):
     def __init__(
         self,
         api_key: str,
         engine: str = os.environ.get("GPT_ENGINE") or "llama3-70b-8192",
         api_url: str = "https://api.groq.com/openai/v1/chat/completions",
```

### Comparing `modelmerge-0.5.5/src/ModelMerge/plugins/image.py` & `modelmerge-0.5.6/src/ModelMerge/plugins/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import requests
 import json
-from ..models.config import BaseLLM
+from ..models.base import BaseLLM
 
 API = os.environ.get('API', None)
 API_URL = os.environ.get('API_URL', None)
 
 class dalle3(BaseLLM):
     def __init__(
         self,
```

### Comparing `modelmerge-0.5.5/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.5.6/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.5.6/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/src/ModelMerge/tools/chatgpt.py` & `modelmerge-0.5.6/src/ModelMerge/tools/chatgpt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/src/ModelMerge/tools/claude.py` & `modelmerge-0.5.6/src/ModelMerge/tools/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/src/ModelMerge/tools/run.py` & `modelmerge-0.5.6/src/ModelMerge/tools/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import os
 import json
 
 from ..utils.scripts import cut_message
 from ..utils.prompt import search_key_word_prompt
 
 from ..plugins import *
-from ..models.config import LANGUAGE
+
+LANGUAGE = os.environ.get('LANGUAGE', 'Simplified Chinese')
 
 
 def get_tools_result(function_call_name, function_full_response, function_call_max_tokens, engine, robot, api_key, api_url, use_plugins):
     if function_call_name == "get_search_results":
         prompt = json.loads(function_full_response)["prompt"]
         yield "🌐 正在搜索您的问题，提取关键词..."
         llm = robot(api_key=api_key, api_url=api_url.source_api_url, engine=engine, use_plugins=use_plugins)
```

### Comparing `modelmerge-0.5.5/src/ModelMerge/utils/prompt.py` & `modelmerge-0.5.6/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/src/ModelMerge/utils/scripts.py` & `modelmerge-0.5.6/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.5.6/src/modelmerge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.5.5
+Version: 0.5.6
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.5.5/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.5.6/src/modelmerge.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 LICENSE
 README.md
 setup.py
 src/ModelMerge/__init__.py
 src/ModelMerge/models/__init__.py
+src/ModelMerge/models/base.py
 src/ModelMerge/models/chatgpt.py
 src/ModelMerge/models/claude.py
-src/ModelMerge/models/config.py
 src/ModelMerge/models/genimi.py
 src/ModelMerge/models/groq.py
 src/ModelMerge/plugins/__init__.py
+src/ModelMerge/plugins/config.py
 src/ModelMerge/plugins/image.py
 src/ModelMerge/plugins/run_python.py
 src/ModelMerge/plugins/tarvel.py
 src/ModelMerge/plugins/today.py
 src/ModelMerge/plugins/version.py
 src/ModelMerge/plugins/websearch.py
 src/ModelMerge/tools/__init__.py
@@ -37,11 +38,12 @@
 test/test_google_search.py
 test/test_jieba.py
 test/test_json.py
 test/test_langchain_search_old.py
 test/test_logging.py
 test/test_ollama.py
 test/test_py_run.py
+test/test_requests.py
 test/test_tikitoken.py
 test/test_token.py
 test/test_url.py
 test/test_whisper.py
```

### Comparing `modelmerge-0.5.5/test/test_Web_crawler.py` & `modelmerge-0.5.6/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/test/test_claude_zh_char.py` & `modelmerge-0.5.6/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/test/test_ddg_search.py` & `modelmerge-0.5.6/test/test_ddg_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/test/test_download_pdf.py` & `modelmerge-0.5.6/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/test/test_get_token_dict.py` & `modelmerge-0.5.6/test/test_get_token_dict.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/test/test_google_search.py` & `modelmerge-0.5.6/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/test/test_jieba.py` & `modelmerge-0.5.6/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/test/test_json.py` & `modelmerge-0.5.6/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/test/test_langchain_search_old.py` & `modelmerge-0.5.6/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/test/test_logging.py` & `modelmerge-0.5.6/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/test/test_py_run.py` & `modelmerge-0.5.6/test/test_py_run.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/test/test_tikitoken.py` & `modelmerge-0.5.6/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/test/test_token.py` & `modelmerge-0.5.6/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.5/test/test_url.py` & `modelmerge-0.5.6/test/test_url.py`

 * *Files identical despite different names*

