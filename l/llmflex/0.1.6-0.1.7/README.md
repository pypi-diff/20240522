# Comparing `tmp/llmflex-0.1.6.tar.gz` & `tmp/llmflex-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmflex-0.1.6.tar", last modified: Tue May 21 17:59:46 2024, max compression
+gzip compressed data, was "llmflex-0.1.7.tar", last modified: Wed May 22 20:09:35 2024, max compression
```

## Comparing `llmflex-0.1.6.tar` & `llmflex-0.1.7.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.289543 llmflex-0.1.6/
--rw-r--r--   0 nathan95   (501) staff       (20)     1067 2024-01-22 01:35:14.000000 llmflex-0.1.6/LICENSE.md
--rw-r--r--   0 nathan95   (501) staff       (20)    10171 2024-05-21 17:59:46.289237 llmflex-0.1.6/PKG-INFO
--rw-r--r--   0 nathan95   (501) staff       (20)     8926 2024-05-21 17:59:14.000000 llmflex-0.1.6/README.md
--rw-r--r--   0 nathan95   (501) staff       (20)     1244 2024-05-21 17:59:14.000000 llmflex-0.1.6/pyproject.toml
--rw-r--r--   0 nathan95   (501) staff       (20)       38 2024-05-21 17:59:46.289610 llmflex-0.1.6/setup.cfg
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.278376 llmflex-0.1.6/src/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.280372 llmflex-0.1.6/src/llmflex/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.282001 llmflex-0.1.6/src/llmflex/Embeddings/
--rw-r--r--   0 nathan95   (501) staff       (20)      226 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Embeddings/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4555 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Embeddings/api_embeddings.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4608 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Embeddings/base_embeddings.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2275 2024-03-15 22:38:26.000000 llmflex-0.1.6/src/llmflex/Embeddings/hf_embeddings_server.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4147 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Embeddings/huggingface_embeddings.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.282454 llmflex-0.1.6/src/llmflex/Frontend/
--rw-r--r--   0 nathan95   (501) staff       (20)      102 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Frontend/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    29992 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Frontend/gradio_interface.py
--rw-r--r--   0 nathan95   (501) staff       (20)    37304 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Frontend/streamlit_interface.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.282741 llmflex-0.1.6/src/llmflex/KnowledgeBase/
--rw-r--r--   0 nathan95   (501) staff       (20)      108 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/KnowledgeBase/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    13135 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/KnowledgeBase/knowledge_base.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.283611 llmflex-0.1.6/src/llmflex/Memory/
--rw-r--r--   0 nathan95   (501) staff       (20)      287 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Memory/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8298 2024-03-11 17:44:28.000000 llmflex-0.1.6/src/llmflex/Memory/assistant_long_term_memory.py
--rw-r--r--   0 nathan95   (501) staff       (20)    13190 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Memory/base_memory.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7727 2024-03-11 17:44:28.000000 llmflex-0.1.6/src/llmflex/Memory/long_short_memory.py
--rw-r--r--   0 nathan95   (501) staff       (20)    13523 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Memory/longshort_memory.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.283819 llmflex-0.1.6/src/llmflex/Models/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.284764 llmflex-0.1.6/src/llmflex/Models/Cores/
--rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Models/Cores/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    15426 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Models/Cores/base_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7915 2024-02-25 22:17:53.000000 llmflex-0.1.6/src/llmflex/Models/Cores/exllamav2_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     9365 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Models/Cores/huggingface_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8223 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Models/Cores/llamacpp_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     9273 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Models/Cores/openai_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7481 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Models/Cores/utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.284987 llmflex-0.1.6/src/llmflex/Models/Factory/
--rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Models/Factory/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    10723 2024-04-14 12:29:06.000000 llmflex-0.1.6/src/llmflex/Models/Factory/llm_factory.py
--rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Models/__init__.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.285267 llmflex-0.1.6/src/llmflex/Prompts/
--rw-r--r--   0 nathan95   (501) staff       (20)       52 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Prompts/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    21647 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Prompts/prompt_template.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.285684 llmflex-0.1.6/src/llmflex/Rankers/
--rw-r--r--   0 nathan95   (501) staff       (20)       81 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Rankers/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1471 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Rankers/base_ranker.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2309 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Rankers/flashrank_ranker.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.286115 llmflex-0.1.6/src/llmflex/Schemas/
--rw-r--r--   0 nathan95   (501) staff       (20)       64 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Schemas/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1414 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Schemas/documents.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2429 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Schemas/tokenizer.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.286753 llmflex-0.1.6/src/llmflex/TextSplitters/
--rw-r--r--   0 nathan95   (501) staff       (20)      123 2024-03-11 17:44:28.000000 llmflex-0.1.6/src/llmflex/TextSplitters/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1526 2024-03-11 17:44:28.000000 llmflex-0.1.6/src/llmflex/TextSplitters/base_text_splitter.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2860 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/TextSplitters/sentence_token_text_splitter.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1423 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/TextSplitters/token_text_splitter.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.287865 llmflex-0.1.6/src/llmflex/Tools/
--rw-r--r--   0 nathan95   (501) staff       (20)      115 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Tools/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    11795 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/Tools/base_tool.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2983 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Tools/browser_tool.py
--rw-r--r--   0 nathan95   (501) staff       (20)       45 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Tools/tool_prompting.py
--rw-r--r--   0 nathan95   (501) staff       (20)     6603 2024-03-11 17:44:28.000000 llmflex-0.1.6/src/llmflex/Tools/tool_selection.py
--rw-r--r--   0 nathan95   (501) staff       (20)     9639 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Tools/tool_utils.py
--rw-r--r--   0 nathan95   (501) staff       (20)    11421 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/Tools/web_search_tool.py
--rw-r--r--   0 nathan95   (501) staff       (20)    15193 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/Tools/web_search_utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.288360 llmflex-0.1.6/src/llmflex/VectorDBs/
--rw-r--r--   0 nathan95   (501) staff       (20)       93 2024-03-11 17:44:28.000000 llmflex-0.1.6/src/llmflex/VectorDBs/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    24488 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/VectorDBs/base_vectordb.py
--rw-r--r--   0 nathan95   (501) staff       (20)     5362 2024-04-21 17:42:51.000000 llmflex-0.1.6/src/llmflex/VectorDBs/faiss_vectordb.py
--rw-r--r--   0 nathan95   (501) staff       (20)      275 2024-05-21 17:59:14.000000 llmflex-0.1.6/src/llmflex/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4381 2024-02-24 22:31:02.000000 llmflex-0.1.6/src/llmflex/cli.py
--rw-r--r--   0 nathan95   (501) staff       (20)     6178 2024-03-11 17:44:28.000000 llmflex-0.1.6/src/llmflex/utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-21 17:59:46.288542 llmflex-0.1.6/src/llmflex.egg-info/
--rw-r--r--   0 nathan95   (501) staff       (20)    10171 2024-05-21 17:59:46.000000 llmflex-0.1.6/src/llmflex.egg-info/PKG-INFO
--rw-r--r--   0 nathan95   (501) staff       (20)     2165 2024-05-21 17:59:46.000000 llmflex-0.1.6/src/llmflex.egg-info/SOURCES.txt
--rw-r--r--   0 nathan95   (501) staff       (20)        1 2024-05-21 17:59:46.000000 llmflex-0.1.6/src/llmflex.egg-info/dependency_links.txt
--rw-r--r--   0 nathan95   (501) staff       (20)       44 2024-05-21 17:59:46.000000 llmflex-0.1.6/src/llmflex.egg-info/entry_points.txt
--rw-r--r--   0 nathan95   (501) staff       (20)      357 2024-05-21 17:59:46.000000 llmflex-0.1.6/src/llmflex.egg-info/requires.txt
--rw-r--r--   0 nathan95   (501) staff       (20)        8 2024-05-21 17:59:46.000000 llmflex-0.1.6/src/llmflex.egg-info/top_level.txt
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.132888 llmflex-0.1.7/
+-rw-r--r--   0 nathan95   (501) staff       (20)     1067 2024-01-22 01:35:14.000000 llmflex-0.1.7/LICENSE.md
+-rw-r--r--   0 nathan95   (501) staff       (20)    10171 2024-05-22 20:09:35.132659 llmflex-0.1.7/PKG-INFO
+-rw-r--r--   0 nathan95   (501) staff       (20)     8926 2024-05-21 17:59:14.000000 llmflex-0.1.7/README.md
+-rw-r--r--   0 nathan95   (501) staff       (20)     1244 2024-05-21 17:59:14.000000 llmflex-0.1.7/pyproject.toml
+-rw-r--r--   0 nathan95   (501) staff       (20)       38 2024-05-22 20:09:35.132941 llmflex-0.1.7/setup.cfg
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.121561 llmflex-0.1.7/src/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.123479 llmflex-0.1.7/src/llmflex/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.125162 llmflex-0.1.7/src/llmflex/Embeddings/
+-rw-r--r--   0 nathan95   (501) staff       (20)      226 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Embeddings/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4555 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Embeddings/api_embeddings.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4608 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Embeddings/base_embeddings.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2275 2024-03-15 22:38:26.000000 llmflex-0.1.7/src/llmflex/Embeddings/hf_embeddings_server.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4147 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Embeddings/huggingface_embeddings.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.125620 llmflex-0.1.7/src/llmflex/Frontend/
+-rw-r--r--   0 nathan95   (501) staff       (20)      102 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Frontend/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    29992 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Frontend/gradio_interface.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    37304 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Frontend/streamlit_interface.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.125927 llmflex-0.1.7/src/llmflex/KnowledgeBase/
+-rw-r--r--   0 nathan95   (501) staff       (20)      108 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/KnowledgeBase/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    13135 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/KnowledgeBase/knowledge_base.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.126841 llmflex-0.1.7/src/llmflex/Memory/
+-rw-r--r--   0 nathan95   (501) staff       (20)      287 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Memory/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     8298 2024-03-11 17:44:28.000000 llmflex-0.1.7/src/llmflex/Memory/assistant_long_term_memory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    13190 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Memory/base_memory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7727 2024-03-11 17:44:28.000000 llmflex-0.1.7/src/llmflex/Memory/long_short_memory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    13523 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Memory/longshort_memory.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.127040 llmflex-0.1.7/src/llmflex/Models/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.128324 llmflex-0.1.7/src/llmflex/Models/Cores/
+-rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Models/Cores/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    15434 2024-05-22 20:08:53.000000 llmflex-0.1.7/src/llmflex/Models/Cores/base_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7915 2024-02-25 22:17:53.000000 llmflex-0.1.7/src/llmflex/Models/Cores/exllamav2_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     9365 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Models/Cores/huggingface_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     8223 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Models/Cores/llamacpp_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     9273 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Models/Cores/openai_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7524 2024-05-22 20:08:53.000000 llmflex-0.1.7/src/llmflex/Models/Cores/utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.128585 llmflex-0.1.7/src/llmflex/Models/Factory/
+-rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Models/Factory/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    10723 2024-04-14 12:29:06.000000 llmflex-0.1.7/src/llmflex/Models/Factory/llm_factory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Models/__init__.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.128919 llmflex-0.1.7/src/llmflex/Prompts/
+-rw-r--r--   0 nathan95   (501) staff       (20)       52 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Prompts/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    21647 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Prompts/prompt_template.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.129330 llmflex-0.1.7/src/llmflex/Rankers/
+-rw-r--r--   0 nathan95   (501) staff       (20)       81 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Rankers/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1471 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Rankers/base_ranker.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2309 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Rankers/flashrank_ranker.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.129710 llmflex-0.1.7/src/llmflex/Schemas/
+-rw-r--r--   0 nathan95   (501) staff       (20)       64 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Schemas/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1414 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Schemas/documents.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2429 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Schemas/tokenizer.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.130214 llmflex-0.1.7/src/llmflex/TextSplitters/
+-rw-r--r--   0 nathan95   (501) staff       (20)      123 2024-03-11 17:44:28.000000 llmflex-0.1.7/src/llmflex/TextSplitters/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1526 2024-03-11 17:44:28.000000 llmflex-0.1.7/src/llmflex/TextSplitters/base_text_splitter.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2860 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/TextSplitters/sentence_token_text_splitter.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1423 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/TextSplitters/token_text_splitter.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.131386 llmflex-0.1.7/src/llmflex/Tools/
+-rw-r--r--   0 nathan95   (501) staff       (20)      115 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Tools/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    11795 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Tools/base_tool.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2983 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Tools/browser_tool.py
+-rw-r--r--   0 nathan95   (501) staff       (20)       45 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Tools/tool_prompting.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     6603 2024-03-11 17:44:28.000000 llmflex-0.1.7/src/llmflex/Tools/tool_selection.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     9639 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Tools/tool_utils.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    11421 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Tools/web_search_tool.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    15193 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Tools/web_search_utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.131838 llmflex-0.1.7/src/llmflex/VectorDBs/
+-rw-r--r--   0 nathan95   (501) staff       (20)       93 2024-03-11 17:44:28.000000 llmflex-0.1.7/src/llmflex/VectorDBs/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    24488 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/VectorDBs/base_vectordb.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     5362 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/VectorDBs/faiss_vectordb.py
+-rw-r--r--   0 nathan95   (501) staff       (20)      275 2024-05-22 20:08:53.000000 llmflex-0.1.7/src/llmflex/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4381 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/cli.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     6178 2024-03-11 17:44:28.000000 llmflex-0.1.7/src/llmflex/utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.132036 llmflex-0.1.7/src/llmflex.egg-info/
+-rw-r--r--   0 nathan95   (501) staff       (20)    10171 2024-05-22 20:09:35.000000 llmflex-0.1.7/src/llmflex.egg-info/PKG-INFO
+-rw-r--r--   0 nathan95   (501) staff       (20)     2165 2024-05-22 20:09:35.000000 llmflex-0.1.7/src/llmflex.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)        1 2024-05-22 20:09:35.000000 llmflex-0.1.7/src/llmflex.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)       44 2024-05-22 20:09:35.000000 llmflex-0.1.7/src/llmflex.egg-info/entry_points.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)      357 2024-05-22 20:09:35.000000 llmflex-0.1.7/src/llmflex.egg-info/requires.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)        8 2024-05-22 20:09:35.000000 llmflex-0.1.7/src/llmflex.egg-info/top_level.txt
```

### Comparing `llmflex-0.1.6/LICENSE.md` & `llmflex-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/PKG-INFO` & `llmflex-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflex
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python package for developing AI applications with local LLMs.
 Author-email: Nathan Tam <nathan1295@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nath1295/LLMFlex
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `llmflex-0.1.6/README.md` & `llmflex-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/pyproject.toml` & `llmflex-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Embeddings/api_embeddings.py` & `llmflex-0.1.7/src/llmflex/Embeddings/api_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Embeddings/base_embeddings.py` & `llmflex-0.1.7/src/llmflex/Embeddings/base_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Embeddings/hf_embeddings_server.py` & `llmflex-0.1.7/src/llmflex/Embeddings/hf_embeddings_server.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Embeddings/huggingface_embeddings.py` & `llmflex-0.1.7/src/llmflex/Embeddings/huggingface_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Frontend/gradio_interface.py` & `llmflex-0.1.7/src/llmflex/Frontend/gradio_interface.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Frontend/streamlit_interface.py` & `llmflex-0.1.7/src/llmflex/Frontend/streamlit_interface.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/KnowledgeBase/knowledge_base.py` & `llmflex-0.1.7/src/llmflex/KnowledgeBase/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Memory/assistant_long_term_memory.py` & `llmflex-0.1.7/src/llmflex/Memory/assistant_long_term_memory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Memory/base_memory.py` & `llmflex-0.1.7/src/llmflex/Memory/base_memory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Memory/long_short_memory.py` & `llmflex-0.1.7/src/llmflex/Memory/long_short_memory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Memory/longshort_memory.py` & `llmflex-0.1.7/src/llmflex/Memory/longshort_memory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Models/Cores/base_core.py` & `llmflex-0.1.7/src/llmflex/Models/Cores/base_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,17 +110,17 @@
     def prompt_template(self) -> PromptTemplate:
         """Default prompt template for the model.
 
         Returns:
             PromptTemplate: Default prompt template for the model.
         """
         if not hasattr(self, '_prompt_template'):
-            from transformers import PreTrainedTokenizer
+            from transformers import PreTrainedTokenizerBase
             from .utils import detect_prompt_template_by_id, get_prompt_template_by_jinja
-            if isinstance(self.tokenizer, PreTrainedTokenizer):
+            if isinstance(self.tokenizer, PreTrainedTokenizerBase):
                 self._prompt_template = get_prompt_template_by_jinja(self.model_id, tokenizer=self.tokenizer)
             elif self.core_type == 'LlamaCppCore':
                 preset = detect_prompt_template_by_id(self.model_id)
                 preset = _chat_formats_map.get(self._model.chat_format, 'Default') if preset == 'Default' else preset
                 self._prompt_template = PromptTemplate.from_preset(preset)
             else:
                 self._prompt_template = PromptTemplate.from_preset(detect_prompt_template_by_id(self.model_id))
```

### Comparing `llmflex-0.1.6/src/llmflex/Models/Cores/exllamav2_core.py` & `llmflex-0.1.7/src/llmflex/Models/Cores/exllamav2_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Models/Cores/huggingface_core.py` & `llmflex-0.1.7/src/llmflex/Models/Cores/huggingface_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Models/Cores/llamacpp_core.py` & `llmflex-0.1.7/src/llmflex/Models/Cores/llamacpp_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Models/Cores/openai_core.py` & `llmflex-0.1.7/src/llmflex/Models/Cores/openai_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Models/Cores/utils.py` & `llmflex-0.1.7/src/llmflex/Models/Cores/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,16 +155,17 @@
     Returns:
         str: Prompt template preset.
     """
     from ...Prompts.prompt_template import presets
     for k, v in presets.items():
         if jinja_template in v['template']:
             return k
-        if all(kw in jinja_template for kw in v['keywords']):
-            return k
+        if 'keywords' in v.keys():
+            if all(kw in jinja_template for kw in v['keywords']):
+                return k
     return 'Default'
 
 def get_prompt_template_by_jinja(model_id: str, tokenizer: Any) -> PromptTemplate:
     """Getting the appropriate prompt template given the huggingface tokenizer.
 
     Args:
         model_id (str): Repo ID of the tokenizer.
```

### Comparing `llmflex-0.1.6/src/llmflex/Models/Factory/llm_factory.py` & `llmflex-0.1.7/src/llmflex/Models/Factory/llm_factory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Prompts/prompt_template.py` & `llmflex-0.1.7/src/llmflex/Prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Rankers/base_ranker.py` & `llmflex-0.1.7/src/llmflex/Rankers/base_ranker.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Rankers/flashrank_ranker.py` & `llmflex-0.1.7/src/llmflex/Rankers/flashrank_ranker.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Schemas/documents.py` & `llmflex-0.1.7/src/llmflex/Schemas/documents.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Schemas/tokenizer.py` & `llmflex-0.1.7/src/llmflex/Schemas/tokenizer.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/TextSplitters/base_text_splitter.py` & `llmflex-0.1.7/src/llmflex/TextSplitters/base_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/TextSplitters/sentence_token_text_splitter.py` & `llmflex-0.1.7/src/llmflex/TextSplitters/sentence_token_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/TextSplitters/token_text_splitter.py` & `llmflex-0.1.7/src/llmflex/TextSplitters/token_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Tools/base_tool.py` & `llmflex-0.1.7/src/llmflex/Tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Tools/browser_tool.py` & `llmflex-0.1.7/src/llmflex/Tools/browser_tool.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Tools/tool_selection.py` & `llmflex-0.1.7/src/llmflex/Tools/tool_selection.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Tools/tool_utils.py` & `llmflex-0.1.7/src/llmflex/Tools/tool_utils.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Tools/web_search_tool.py` & `llmflex-0.1.7/src/llmflex/Tools/web_search_tool.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/Tools/web_search_utils.py` & `llmflex-0.1.7/src/llmflex/Tools/web_search_utils.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/VectorDBs/base_vectordb.py` & `llmflex-0.1.7/src/llmflex/VectorDBs/base_vectordb.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/VectorDBs/faiss_vectordb.py` & `llmflex-0.1.7/src/llmflex/VectorDBs/faiss_vectordb.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/cli.py` & `llmflex-0.1.7/src/llmflex/cli.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex/utils.py` & `llmflex-0.1.7/src/llmflex/utils.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.6/src/llmflex.egg-info/PKG-INFO` & `llmflex-0.1.7/src/llmflex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflex
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python package for developing AI applications with local LLMs.
 Author-email: Nathan Tam <nathan1295@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nath1295/LLMFlex
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `llmflex-0.1.6/src/llmflex.egg-info/SOURCES.txt` & `llmflex-0.1.7/src/llmflex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

