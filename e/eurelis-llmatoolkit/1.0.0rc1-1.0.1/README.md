# Comparing `tmp/eurelis_llmatoolkit-1.0.0rc1.tar.gz` & `tmp/eurelis_llmatoolkit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurelis_llmatoolkit-1.0.0rc1.tar", last modified: Thu May 16 18:31:52 2024, max compression
+gzip compressed data, was "eurelis_llmatoolkit-1.0.1.tar", last modified: Wed May 22 12:14:42 2024, max compression
```

## Comparing `eurelis_llmatoolkit-1.0.0rc1.tar` & `eurelis_llmatoolkit-1.0.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.186884 eurelis_llmatoolkit-1.0.0rc1/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1064 2024-04-27 08:12:19.000000 eurelis_llmatoolkit-1.0.0rc1/LICENSE
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2254 2024-05-16 18:31:52.185482 eurelis_llmatoolkit-1.0.0rc1/PKG-INFO
--rw-r--r--   0 vincentlambert   (501) staff       (20)      424 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/README.md
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1551 2024-05-16 18:23:41.000000 eurelis_llmatoolkit-1.0.0rc1/pyproject.toml
--rw-r--r--   0 vincentlambert   (501) staff       (20)       38 2024-05-16 18:31:52.187170 eurelis_llmatoolkit-1.0.0rc1/setup.cfg
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.109037 eurelis_llmatoolkit-1.0.0rc1/src/
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.126157 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.134194 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3930 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.138058 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/acronyms/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1530 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/acronyms/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1996 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/acronyms/acronyms_chain_wrapper.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2055 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/acronyms/acronyms_document_transformer.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)      654 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/acronyms/acronyms_text_transformer.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.139210 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/addons/
--rw-r--r--   0 vincentlambert   (501) staff       (20)        0 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/addons/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.143261 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/addons/checker/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      207 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/addons/checker/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2110 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/addons/checker/chat_checker.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)      428 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/addons/checker/check_input.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1621 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/addons/checker/check_input_callback.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)        0 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/addons/checker/method.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.143986 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/addons/output/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1648 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/addons/output/markdown_html_callback.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.145052 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/chains/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      615 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/chains/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.145957 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/chains/conversational_retrieval/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     6601 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/chains/conversational_retrieval/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     5414 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/console.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.147852 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/dataset/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     6886 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/dataset/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)    12678 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/dataset/dataset.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.149160 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      622 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.150052 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/fs/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2552 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/fs/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.151772 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/list/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2571 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/list/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2371 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/list/list_loader.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.152818 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/sitemap/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3139 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/sitemap/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.153765 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/url/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2133 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/url/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.155615 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_transformers/
--rw-r--r--   0 vincentlambert   (501) staff       (20)        0 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_transformers/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1301 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_transformers/base.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.156600 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_transformers/html2text/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      796 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_transformers/html2text/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.157535 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_transformers/urloutput/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3530 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_transformers/urloutput/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.158699 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/embeddings/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      614 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/embeddings/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.159678 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/embeddings/huggingface/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      846 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/embeddings/huggingface/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.160496 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/embeddings/openai/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1309 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/embeddings/openai/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2922 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/gradiochat.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)    30485 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/langchain_wrapper.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.161648 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/llms/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      419 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/llms/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.162262 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/llms/huggingface/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      996 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/llms/huggingface/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.163050 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/llms/openai/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2470 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/llms/openai/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.164510 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/memory/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      548 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/memory/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1008 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/memory/conversation_buffer_memory.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.165967 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/parsers/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1267 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/parsers/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1230 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/parsers/pdf.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.166632 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/retrievers/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      516 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/retrievers/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.167413 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/retrievers/selfquery/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2053 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/retrievers/selfquery/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.168045 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/retrievers/vectorstore/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      890 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/retrievers/vectorstore/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.169133 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/text_splitters/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     4078 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/text_splitters/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.170093 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/text_transformers/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      366 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/text_transformers/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.170773 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/vectorstores/
--rw-r--r--   0 vincentlambert   (501) staff       (20)      579 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/vectorstores/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.171481 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/vectorstores/chroma/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3119 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/vectorstores/chroma/__init__.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.173274 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/vectorstores/mongodb/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3825 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/vectorstores/mongodb/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2423 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/vectorstores/mongodb/mongodb_similarity_atlas_vector_store_search.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.173915 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/vectorstores/solr/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1195 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/vectorstores/solr/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)      612 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/types.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.177089 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     6892 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/base_factory.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     9747 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/class_loader.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1425 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/misc.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.180976 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/output/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2638 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/output/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3460 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/output/base_console_output.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3696 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/output/logging_console_output.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)      755 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/output/output.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1418 2024-05-16 17:18:54.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/output/verbose_console_output.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:31:52.181762 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit.egg-info/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2254 2024-05-16 18:31:52.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit.egg-info/PKG-INFO
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3874 2024-05-16 18:31:52.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 vincentlambert   (501) staff       (20)        1 2024-05-16 18:31:52.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 vincentlambert   (501) staff       (20)       79 2024-05-16 18:31:52.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit.egg-info/entry_points.txt
--rw-r--r--   0 vincentlambert   (501) staff       (20)      520 2024-05-16 18:31:52.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit.egg-info/requires.txt
--rw-r--r--   0 vincentlambert   (501) staff       (20)       20 2024-05-16 18:31:52.000000 eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.178556 eurelis_llmatoolkit-1.0.1/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1064 2024-04-27 08:12:19.000000 eurelis_llmatoolkit-1.0.1/LICENSE
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2251 2024-05-22 12:14:42.177607 eurelis_llmatoolkit-1.0.1/PKG-INFO
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      424 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/README.md
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1548 2024-05-22 12:13:49.000000 eurelis_llmatoolkit-1.0.1/pyproject.toml
+-rw-r--r--   0 vincentlambert   (501) staff       (20)       38 2024-05-22 12:14:42.178730 eurelis_llmatoolkit-1.0.1/setup.cfg
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.111614 eurelis_llmatoolkit-1.0.1/src/
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.126695 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.134906 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3930 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.138280 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/acronyms/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1530 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/acronyms/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1996 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/acronyms/acronyms_chain_wrapper.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2055 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/acronyms/acronyms_document_transformer.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      654 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/acronyms/acronyms_text_transformer.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.138974 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/addons/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/addons/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.142905 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/addons/checker/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      207 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/addons/checker/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2110 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/addons/checker/chat_checker.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      428 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/addons/checker/check_input.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1621 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/addons/checker/check_input_callback.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/addons/checker/method.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.143507 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/addons/output/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1648 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/addons/output/markdown_html_callback.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.144145 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/chains/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      615 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/chains/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.144734 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/chains/conversational_retrieval/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     6601 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/chains/conversational_retrieval/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     5449 2024-05-20 17:18:12.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/console.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.146029 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/dataset/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     6886 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/dataset/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)    12678 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/dataset/dataset.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.146679 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      622 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.147236 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/fs/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2552 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/fs/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.148745 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/list/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2571 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/list/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2371 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/list/list_loader.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.149550 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/sitemap/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3170 2024-05-22 12:13:49.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/sitemap/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.150164 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/url/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2133 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/url/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.151580 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_transformers/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)        0 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_transformers/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1301 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_transformers/base.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.152750 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_transformers/html2text/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      796 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_transformers/html2text/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.153508 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_transformers/urloutput/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3530 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_transformers/urloutput/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.154005 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/embeddings/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      614 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/embeddings/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.154540 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/embeddings/huggingface/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      846 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/embeddings/huggingface/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.155237 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/embeddings/openai/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1309 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/embeddings/openai/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2922 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/gradiochat.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)    30485 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/langchain_wrapper.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.155837 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/llms/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      419 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/llms/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.156513 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/llms/huggingface/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      996 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/llms/huggingface/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.157437 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/llms/openai/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2470 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/llms/openai/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.158914 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/memory/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      548 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/memory/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1008 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/memory/conversation_buffer_memory.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.160305 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/parsers/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1267 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/parsers/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1230 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/parsers/pdf.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.160898 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/retrievers/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      516 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/retrievers/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.161582 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/retrievers/selfquery/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2053 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/retrievers/selfquery/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.162314 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/retrievers/vectorstore/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      890 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/retrievers/vectorstore/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.163013 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/text_splitters/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     4078 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/text_splitters/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.163703 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/text_transformers/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      366 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/text_transformers/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.164391 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/vectorstores/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      579 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/vectorstores/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.165237 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/vectorstores/chroma/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3119 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/vectorstores/chroma/__init__.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.166719 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/vectorstores/mongodb/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3825 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/vectorstores/mongodb/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2423 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/vectorstores/mongodb/mongodb_similarity_atlas_vector_store_search.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.167565 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/vectorstores/solr/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1312 2024-05-22 12:13:49.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/vectorstores/solr/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      612 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/types.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.170260 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     6892 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/base_factory.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     9747 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/class_loader.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1425 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/misc.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.173749 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/output/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2638 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/output/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3460 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/output/base_console_output.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3696 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/output/logging_console_output.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      755 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/output/output.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1418 2024-05-16 18:33:18.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/output/verbose_console_output.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-22 12:14:42.174729 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit.egg-info/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2251 2024-05-22 12:14:42.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3874 2024-05-22 12:14:42.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 vincentlambert   (501) staff       (20)        1 2024-05-22 12:14:42.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 vincentlambert   (501) staff       (20)       79 2024-05-22 12:14:42.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit.egg-info/entry_points.txt
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      520 2024-05-22 12:14:42.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit.egg-info/requires.txt
+-rw-r--r--   0 vincentlambert   (501) staff       (20)       20 2024-05-22 12:14:42.000000 eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit.egg-info/top_level.txt
```

### Comparing `eurelis_llmatoolkit-1.0.0rc1/LICENSE` & `eurelis_llmatoolkit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/PKG-INFO` & `eurelis_llmatoolkit-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eurelis_llmatoolkit
-Version: 1.0.0rc1
+Name: eurelis-llmatoolkit
+Version: 1.0.1
 Summary: Framework to build and manage IA based applications. Based on Langchain under the hood.
 Author-email: Vincent LAMBERT <v.lambert@eurelis.com>, Jérôme DIAZ <j.diaz@eurelis.com>
 Project-URL: Homepage, https://github.com/Eurelis/Eurelis-LlmaToolkit
 Project-URL: Bug Tracker, https://github.com/Eurelis/Eurelis-LlmaToolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -19,15 +19,15 @@
 Requires-Dist: numpy==1.26.0
 Provides-Extra: huggingface
 Requires-Dist: sentence_transformers==2.2.2; extra == "huggingface"
 Requires-Dist: transformers==4.34.1; extra == "huggingface"
 Provides-Extra: openai
 Requires-Dist: langchain-openai==0.0.2.post1; extra == "openai"
 Provides-Extra: solr
-Requires-Dist: eurelis-langchain-solr-vectorstore==0.0.1; extra == "solr"
+Requires-Dist: eurelis-langchain-solr-vectorstore==0.0.3; extra == "solr"
 Provides-Extra: chroma
 Requires-Dist: chromadb==0.4.13; extra == "chroma"
 Provides-Extra: sitemap
 Requires-Dist: lxml==4.9.3; extra == "sitemap"
 Requires-Dist: beautifulsoup4==4.12.2; extra == "sitemap"
 Provides-Extra: chatbot
 Requires-Dist: gradio==3.47.1; extra == "chatbot"
```

### Comparing `eurelis_llmatoolkit-1.0.0rc1/pyproject.toml` & `eurelis_llmatoolkit-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "eurelis_llmatoolkit"
-version = "1.0.0rc1"
+name = "eurelis-llmatoolkit"
+version = "1.0.1"
 authors = [
   { name="Vincent LAMBERT", email="v.lambert@eurelis.com" },
   { name="Jérôme DIAZ", email="j.diaz@eurelis.com" }
 ]
 description = "Framework to build and manage IA based applications. Based on Langchain under the hood."
 readme = "README.md"
 requires-python = ">=3.11"
@@ -31,15 +31,15 @@
     "sentence_transformers==2.2.2",
     "transformers==4.34.1"
 ]
 openai = [
     "langchain-openai==0.0.2.post1",
 ]
 solr = [
-    "eurelis-langchain-solr-vectorstore==0.0.1"
+    "eurelis-langchain-solr-vectorstore==0.0.3"
 ]
 chroma = [
     "chromadb==0.4.13"
 ]
 sitemap = [
     "lxml==4.9.3",
     "beautifulsoup4==4.12.2"
```

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/acronyms/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/acronyms/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/acronyms/acronyms_chain_wrapper.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/acronyms/acronyms_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/acronyms/acronyms_document_transformer.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/acronyms/acronyms_document_transformer.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/acronyms/acronyms_text_transformer.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/acronyms/acronyms_text_transformer.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/addons/checker/chat_checker.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/addons/checker/chat_checker.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/addons/checker/check_input_callback.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/addons/checker/check_input_callback.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/addons/output/markdown_html_callback.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/addons/output/markdown_html_callback.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/chains/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/chains/conversational_retrieval/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/chains/conversational_retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/console.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from eurelis_llmatoolkit.utils.output import Verbosity
 
 if TYPE_CHECKING:
     from eurelis_llmatoolkit.langchain.langchain_wrapper import LangchainWrapper
 
 
+# FIXME: Move to TOP level package
 @click.group()
 @click.option("--verbose/--no-verbose", default=False)
 @click.option("-config", default=None)
 @click.pass_context
 def cli(ctx, **kwargs):
     """
     Root command, will handle retrieving verbose and config options values
```

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/dataset/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/dataset/dataset.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/fs/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/list/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/list/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/list/list_loader.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/list/list_loader.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/sitemap/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/sitemap/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 class SitemapDocumentLoaderFactory(ParamsDictFactory[BaseLoader]):
     OPTIONAL_PARAMS = {
         "filter_urls",
         "blocksize",
         "is_local",
         "continue_on_failure",
         "restrict_to_same_domain",
+        "requests_per_second",
     }
 
     def build(self, context: "BaseContext") -> BaseLoader:
         """
         Construct the sitemap document loader
 
         Args:
```

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_loaders/url/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_loaders/url/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_transformers/base.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_transformers/base.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_transformers/html2text/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_transformers/html2text/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/document_transformers/urloutput/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/document_transformers/urloutput/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/embeddings/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/embeddings/huggingface/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/embeddings/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/embeddings/openai/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/embeddings/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/gradiochat.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/gradiochat.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/langchain_wrapper.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/langchain_wrapper.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/llms/huggingface/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/llms/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/llms/openai/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/llms/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/memory/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/memory/conversation_buffer_memory.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/memory/conversation_buffer_memory.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/parsers/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/parsers/pdf.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/parsers/pdf.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/retrievers/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/retrievers/selfquery/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/retrievers/selfquery/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/retrievers/vectorstore/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/retrievers/vectorstore/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/text_splitters/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/text_splitters/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/vectorstores/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/vectorstores/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/vectorstores/chroma/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/vectorstores/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/vectorstores/mongodb/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/vectorstores/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/vectorstores/mongodb/mongodb_similarity_atlas_vector_store_search.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/vectorstores/mongodb/mongodb_similarity_atlas_vector_store_search.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/langchain/vectorstores/solr/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/langchain/vectorstores/solr/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,23 @@
 
 
 class SolrFactory(ParamsDictFactory[VectorStore]):
     """
     Factory to get a solr based vector store
     """
 
-    OPTIONAL_PARAMS = {"page_content_field", "vector_field", "core_name", "url_base"}
+    OPTIONAL_PARAMS = {
+        "page_content_field",
+        "vector_field",
+        "core_name",
+        "url_base",
+        "query_handler",
+        "update_handler",
+        "metadata_fields",
+    }
 
     def build(self, context: "BaseContext") -> VectorStore:
         """
         Construct a solr based vector store
 
         Args:
             context: the context object, usually the current langchain wrapper instance
```

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/types.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/types.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/base_factory.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/base_factory.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/class_loader.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/class_loader.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/misc.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/misc.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/output/__init__.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/output/__init__.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/output/base_console_output.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/output/base_console_output.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/output/logging_console_output.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/output/logging_console_output.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/output/output.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/output/output.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit/utils/output/verbose_console_output.py` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit/utils/output/verbose_console_output.py`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit.egg-info/PKG-INFO` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eurelis_llmatoolkit
-Version: 1.0.0rc1
+Name: eurelis-llmatoolkit
+Version: 1.0.1
 Summary: Framework to build and manage IA based applications. Based on Langchain under the hood.
 Author-email: Vincent LAMBERT <v.lambert@eurelis.com>, Jérôme DIAZ <j.diaz@eurelis.com>
 Project-URL: Homepage, https://github.com/Eurelis/Eurelis-LlmaToolkit
 Project-URL: Bug Tracker, https://github.com/Eurelis/Eurelis-LlmaToolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -19,15 +19,15 @@
 Requires-Dist: numpy==1.26.0
 Provides-Extra: huggingface
 Requires-Dist: sentence_transformers==2.2.2; extra == "huggingface"
 Requires-Dist: transformers==4.34.1; extra == "huggingface"
 Provides-Extra: openai
 Requires-Dist: langchain-openai==0.0.2.post1; extra == "openai"
 Provides-Extra: solr
-Requires-Dist: eurelis-langchain-solr-vectorstore==0.0.1; extra == "solr"
+Requires-Dist: eurelis-langchain-solr-vectorstore==0.0.3; extra == "solr"
 Provides-Extra: chroma
 Requires-Dist: chromadb==0.4.13; extra == "chroma"
 Provides-Extra: sitemap
 Requires-Dist: lxml==4.9.3; extra == "sitemap"
 Requires-Dist: beautifulsoup4==4.12.2; extra == "sitemap"
 Provides-Extra: chatbot
 Requires-Dist: gradio==3.47.1; extra == "chatbot"
```

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit.egg-info/SOURCES.txt` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eurelis_llmatoolkit-1.0.0rc1/src/eurelis_llmatoolkit.egg-info/requires.txt` & `eurelis_llmatoolkit-1.0.1/src/eurelis_llmatoolkit.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 lark==1.1.8
 
 [sitemap]
 lxml==4.9.3
 beautifulsoup4==4.12.2
 
 [solr]
-eurelis-langchain-solr-vectorstore==0.0.1
+eurelis-langchain-solr-vectorstore==0.0.3
```

