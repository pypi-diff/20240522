# Comparing `tmp/langchain_xiao-0.0.4.tar.gz` & `tmp/langchain_xiao-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_xiao-0.0.4.tar", last modified: Thu May 16 06:58:12 2024, max compression
+gzip compressed data, was "langchain_xiao-0.0.5.tar", last modified: Wed May 22 12:47:28 2024, max compression
```

## Comparing `langchain_xiao-0.0.4.tar` & `langchain_xiao-0.0.5.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 06:58:12.137027 langchain_xiao-0.0.4/
--rw-rw-rw-   0        0        0     3237 2024-04-25 13:48:27.000000 langchain_xiao-0.0.4/.gitignore
--rw-rw-rw-   0        0        0     1087 2024-04-25 12:15:59.000000 langchain_xiao-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      949 2024-05-16 06:58:12.136027 langchain_xiao-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       87 2024-04-26 09:06:01.000000 langchain_xiao-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 06:58:12.072405 langchain_xiao-0.0.4/langchain_xiao/
--rw-rw-rw-   0        0        0       23 2024-05-16 06:56:13.000000 langchain_xiao-0.0.4/langchain_xiao/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 06:58:12.104914 langchain_xiao-0.0.4/langchain_xiao/chat_models/
--rw-rw-rw-   0        0        0      102 2024-05-15 09:01:59.000000 langchain_xiao-0.0.4/langchain_xiao/chat_models/__init__.py
--rw-rw-rw-   0        0        0      755 2024-04-26 08:47:54.000000 langchain_xiao-0.0.4/langchain_xiao/chat_models/baichuan.py
--rw-rw-rw-   0        0        0     5452 2024-05-16 06:55:37.000000 langchain_xiao-0.0.4/langchain_xiao/chat_models/cyou.py
--rw-rw-rw-   0        0        0    14067 2024-04-26 08:47:54.000000 langchain_xiao-0.0.4/langchain_xiao/chat_models/llamacpp.py
--rw-rw-rw-   0        0        0     1235 2024-05-15 09:01:26.000000 langchain_xiao-0.0.4/langchain_xiao/chat_models/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-16 06:58:12.112486 langchain_xiao-0.0.4/langchain_xiao/embeddings/
--rw-rw-rw-   0        0        0       40 2024-04-26 08:47:54.000000 langchain_xiao-0.0.4/langchain_xiao/embeddings/__init__.py
--rw-rw-rw-   0        0        0     2376 2024-04-26 08:47:54.000000 langchain_xiao-0.0.4/langchain_xiao/embeddings/fastllm.py
-drwxrwxrwx   0        0        0        0 2024-05-16 06:58:12.121515 langchain_xiao-0.0.4/langchain_xiao/llms/
--rw-rw-rw-   0        0        0       32 2024-04-26 08:47:54.000000 langchain_xiao-0.0.4/langchain_xiao/llms/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-26 08:47:54.000000 langchain_xiao-0.0.4/langchain_xiao/llms/gpt4all.py
--rw-rw-rw-   0        0        0     1115 2024-04-26 08:50:58.000000 langchain_xiao-0.0.4/langchain_xiao/llms/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-16 06:58:12.122033 langchain_xiao-0.0.4/langchain_xiao/retrievers/
--rw-rw-rw-   0        0        0        0 2024-04-26 08:47:54.000000 langchain_xiao-0.0.4/langchain_xiao/retrievers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 06:58:12.129027 langchain_xiao-0.0.4/langchain_xiao/retrievers/document_compressors/
--rw-rw-rw-   0        0        0       45 2024-04-26 08:47:54.000000 langchain_xiao-0.0.4/langchain_xiao/retrievers/document_compressors/__init__.py
--rw-rw-rw-   0        0        0     3212 2024-04-26 08:47:54.000000 langchain_xiao-0.0.4/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py
-drwxrwxrwx   0        0        0        0 2024-05-16 06:58:12.135027 langchain_xiao-0.0.4/langchain_xiao.egg-info/
--rw-rw-rw-   0        0        0      949 2024-05-16 06:58:11.000000 langchain_xiao-0.0.4/langchain_xiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      892 2024-05-16 06:58:12.000000 langchain_xiao-0.0.4/langchain_xiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 06:58:11.000000 langchain_xiao-0.0.4/langchain_xiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-05-16 06:58:11.000000 langchain_xiao-0.0.4/langchain_xiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-16 06:58:11.000000 langchain_xiao-0.0.4/langchain_xiao.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2024-04-26 08:56:51.000000 langchain_xiao-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       70 2024-04-25 13:09:39.000000 langchain_xiao-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 06:58:12.137027 langchain_xiao-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-16 06:58:12.134027 langchain_xiao-0.0.4/tests/
--rw-rw-rw-   0        0        0     1040 2024-05-15 10:33:19.000000 langchain_xiao-0.0.4/tests/chat_models_utils.py
--rw-rw-rw-   0        0        0      461 2024-04-26 08:50:58.000000 langchain_xiao-0.0.4/tests/fastllm_embeddings.py
--rw-rw-rw-   0        0        0      706 2024-04-26 08:50:58.000000 langchain_xiao-0.0.4/tests/fastllm_rerank.py
--rw-rw-rw-   0        0        0      495 2024-04-26 08:50:58.000000 langchain_xiao-0.0.4/tests/llms_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.807890 langchain_xiao-0.0.5/
+-rw-rw-rw-   0        0        0     3237 2024-04-25 13:48:27.000000 langchain_xiao-0.0.5/.gitignore
+-rw-rw-rw-   0        0        0     1087 2024-04-25 12:15:59.000000 langchain_xiao-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      949 2024-05-22 12:47:28.806889 langchain_xiao-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2024-04-26 09:06:01.000000 langchain_xiao-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.684379 langchain_xiao-0.0.5/langchain_xiao/
+-rw-rw-rw-   0        0        0       23 2024-05-22 12:45:04.000000 langchain_xiao-0.0.5/langchain_xiao/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.749889 langchain_xiao-0.0.5/langchain_xiao/chat_models/
+-rw-rw-rw-   0        0        0      136 2024-05-22 12:26:31.000000 langchain_xiao-0.0.5/langchain_xiao/chat_models/__init__.py
+-rw-rw-rw-   0        0        0      755 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/chat_models/baichuan.py
+-rw-rw-rw-   0        0        0     5452 2024-05-16 06:55:37.000000 langchain_xiao-0.0.5/langchain_xiao/chat_models/cyou.py
+-rw-rw-rw-   0        0        0     9747 2024-05-22 12:40:27.000000 langchain_xiao-0.0.5/langchain_xiao/chat_models/hunyuan.py
+-rw-rw-rw-   0        0        0    14067 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/chat_models/llamacpp.py
+-rw-rw-rw-   0        0        0     1255 2024-05-22 12:27:18.000000 langchain_xiao-0.0.5/langchain_xiao/chat_models/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.751890 langchain_xiao-0.0.5/langchain_xiao/embeddings/
+-rw-rw-rw-   0        0        0       40 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     2376 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/embeddings/fastllm.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.791890 langchain_xiao-0.0.5/langchain_xiao/llms/
+-rw-rw-rw-   0        0        0       32 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/llms/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/llms/gpt4all.py
+-rw-rw-rw-   0        0        0     1115 2024-04-26 08:50:58.000000 langchain_xiao-0.0.5/langchain_xiao/llms/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.798890 langchain_xiao-0.0.5/langchain_xiao/retrievers/
+-rw-rw-rw-   0        0        0        0 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/retrievers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.799890 langchain_xiao-0.0.5/langchain_xiao/retrievers/document_compressors/
+-rw-rw-rw-   0        0        0       45 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/retrievers/document_compressors/__init__.py
+-rw-rw-rw-   0        0        0     3212 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.805889 langchain_xiao-0.0.5/langchain_xiao.egg-info/
+-rw-rw-rw-   0        0        0      949 2024-05-22 12:47:28.000000 langchain_xiao-0.0.5/langchain_xiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      930 2024-05-22 12:47:28.000000 langchain_xiao-0.0.5/langchain_xiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 12:47:28.000000 langchain_xiao-0.0.5/langchain_xiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-22 12:47:28.000000 langchain_xiao-0.0.5/langchain_xiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-22 12:47:28.000000 langchain_xiao-0.0.5/langchain_xiao.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2024-04-26 08:56:51.000000 langchain_xiao-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       70 2024-04-25 13:09:39.000000 langchain_xiao-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 12:47:28.807890 langchain_xiao-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.804890 langchain_xiao-0.0.5/tests/
+-rw-rw-rw-   0        0        0     1255 2024-05-22 12:38:55.000000 langchain_xiao-0.0.5/tests/chat_models_utils.py
+-rw-rw-rw-   0        0        0      461 2024-04-26 08:50:58.000000 langchain_xiao-0.0.5/tests/fastllm_embeddings.py
+-rw-rw-rw-   0        0        0      706 2024-04-26 08:50:58.000000 langchain_xiao-0.0.5/tests/fastllm_rerank.py
+-rw-rw-rw-   0        0        0      495 2024-04-26 08:50:58.000000 langchain_xiao-0.0.5/tests/llms_utils.py
```

### Comparing `langchain_xiao-0.0.4/.gitignore` & `langchain_xiao-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.4/LICENSE` & `langchain_xiao-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.4/PKG-INFO` & `langchain_xiao-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-xiao
-Version: 0.0.4
+Version: 0.0.5
 Summary: langchain extension python package
 Author-email: xiaojinli <553555614@qq.com>
 License: MIT
 Project-URL: Documentation, https://github.com/xiaojinlii/langchain-xiao/blob/main/README.md
 Project-URL: Source, https://github.com/xiaojinlii/langchain-xiao
 Keywords: langchain
 Classifier: Programming Language :: Python :: 3
```

### Comparing `langchain_xiao-0.0.4/langchain_xiao/chat_models/baichuan.py` & `langchain_xiao-0.0.5/langchain_xiao/chat_models/baichuan.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.4/langchain_xiao/chat_models/cyou.py` & `langchain_xiao-0.0.5/langchain_xiao/chat_models/cyou.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.4/langchain_xiao/chat_models/llamacpp.py` & `langchain_xiao-0.0.5/langchain_xiao/chat_models/llamacpp.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.4/langchain_xiao/chat_models/utils.py` & `langchain_xiao-0.0.5/langchain_xiao/chat_models/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from langchain_core.language_models import BaseChatModel
 
 
 XIAO_CHAT_MODELS = [
     "ChatLlamaCpp",
     "MyChatBaichuan",
+    "ChatHunyuan",
     "ChatCyou"
 ]
 
 
 def get_chat_model(instance_type: str, **model_kwargs: Any) -> BaseChatModel:
     if instance_type == "ChatOpenAI":
         try:
```

### Comparing `langchain_xiao-0.0.4/langchain_xiao/embeddings/fastllm.py` & `langchain_xiao-0.0.5/langchain_xiao/embeddings/fastllm.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.4/langchain_xiao/llms/gpt4all.py` & `langchain_xiao-0.0.5/langchain_xiao/llms/gpt4all.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.4/langchain_xiao/llms/utils.py` & `langchain_xiao-0.0.5/langchain_xiao/llms/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.4/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py` & `langchain_xiao-0.0.5/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.4/langchain_xiao.egg-info/PKG-INFO` & `langchain_xiao-0.0.5/langchain_xiao.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-xiao
-Version: 0.0.4
+Version: 0.0.5
 Summary: langchain extension python package
 Author-email: xiaojinli <553555614@qq.com>
 License: MIT
 Project-URL: Documentation, https://github.com/xiaojinlii/langchain-xiao/blob/main/README.md
 Project-URL: Source, https://github.com/xiaojinlii/langchain-xiao
 Keywords: langchain
 Classifier: Programming Language :: Python :: 3
```

### Comparing `langchain_xiao-0.0.4/langchain_xiao.egg-info/SOURCES.txt` & `langchain_xiao-0.0.5/langchain_xiao.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 langchain_xiao.egg-info/SOURCES.txt
 langchain_xiao.egg-info/dependency_links.txt
 langchain_xiao.egg-info/requires.txt
 langchain_xiao.egg-info/top_level.txt
 langchain_xiao/chat_models/__init__.py
 langchain_xiao/chat_models/baichuan.py
 langchain_xiao/chat_models/cyou.py
+langchain_xiao/chat_models/hunyuan.py
 langchain_xiao/chat_models/llamacpp.py
 langchain_xiao/chat_models/utils.py
 langchain_xiao/embeddings/__init__.py
 langchain_xiao/embeddings/fastllm.py
 langchain_xiao/llms/__init__.py
 langchain_xiao/llms/gpt4all.py
 langchain_xiao/llms/utils.py
```

### Comparing `langchain_xiao-0.0.4/pyproject.toml` & `langchain_xiao-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.4/tests/fastllm_rerank.py` & `langchain_xiao-0.0.5/tests/fastllm_rerank.py`

 * *Files identical despite different names*

