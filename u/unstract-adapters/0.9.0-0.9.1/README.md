# Comparing `tmp/unstract_adapters-0.9.0.tar.gz` & `tmp/unstract_adapters-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstract_adapters-0.9.0.tar", last modified: Fri Apr 12 05:09:57 2024, max compression
+gzip compressed data, was "unstract_adapters-0.9.1.tar", last modified: Tue Apr 16 05:29:10 2024, max compression
```

## Comparing `unstract_adapters-0.9.0.tar` & `unstract_adapters-0.9.1.tar`

### file list

```diff
@@ -1,153 +1,153 @@
--rw-r--r--   0        0        0    34523 2024-04-12 05:09:37.376570 unstract_adapters-0.9.0/LICENSE
--rw-r--r--   0        0        0      849 2024-04-12 05:09:37.376570 unstract_adapters-0.9.0/README.md
--rw-r--r--   0        0        0     2632 2024-04-12 05:09:57.816741 unstract_adapters-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      298 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/__init__.py
--rw-r--r--   0        0        0     2805 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/adapterkit.py
--rw-r--r--   0        0        0     1830 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/base.py
--rw-r--r--   0        0        0      282 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/constants.py
--rw-r--r--   0        0        0      183 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/__init__.py
--rw-r--r--   0        0        0      154 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/azure_open_ai/README.md
--rw-r--r--   0        0        0      494 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/azure_open_ai/pyproject.toml
--rw-r--r--   0        0        0      216 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/azure_open_ai/src/__init__.py
--rw-r--r--   0        0        0     2468 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py
--rw-r--r--   0        0        0     1548 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0     1145 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/embedding_adapter.py
--rw-r--r--   0        0        0     1319 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/helper.py
--rw-r--r--   0        0        0       42 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/hugging_face/README.md
--rw-r--r--   0        0        0      491 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/hugging_face/pyproject.toml
--rw-r--r--   0        0        0      216 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/hugging_face/src/__init__.py
--rw-r--r--   0        0        0     2449 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py
--rw-r--r--   0        0        0      940 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json
--rw-r--r--   0        0        0       30 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/open_ai/README.md
--rw-r--r--   0        0        0      482 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/open_ai/pyproject.toml
--rw-r--r--   0        0        0      190 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/open_ai/src/__init__.py
--rw-r--r--   0        0        0     2055 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/open_ai/src/open_ai.py
--rw-r--r--   0        0        0      719 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0       35 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/palm/README.md
--rw-r--r--   0        0        0      476 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/palm/pyproject.toml
--rw-r--r--   0        0        0      179 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/palm/src/__init__.py
--rw-r--r--   0        0        0     1993 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/palm/src/palm.py
--rw-r--r--   0        0        0      804 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/palm/src/static/json_schema.json
--rw-r--r--   0        0        0       46 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/qdrant_fast_embed/README.md
--rw-r--r--   0        0        0      500 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/qdrant_fast_embed/pyproject.toml
--rw-r--r--   0        0        0      240 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/__init__.py
--rw-r--r--   0        0        0     1784 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py
--rw-r--r--   0        0        0      553 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json
--rw-r--r--   0        0        0     2086 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/register.py
--rw-r--r--   0        0        0      184 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/enums.py
--rw-r--r--   0        0        0      502 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/exceptions.py
--rw-r--r--   0        0        0      165 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/__init__.py
--rw-r--r--   0        0        0       33 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/anthropic/README.md
--rw-r--r--   0        0        0      474 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/anthropic/pyproject.toml
--rw-r--r--   0        0        0      207 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/anthropic/src/__init__.py
--rw-r--r--   0        0        0     2000 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/anthropic/src/anthropic.py
--rw-r--r--   0        0        0     1017 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/anthropic/src/static/json_schema.json
--rw-r--r--   0        0        0       33 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/any_scale/README.md
--rw-r--r--   0        0        0      473 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/any_scale/pyproject.toml
--rw-r--r--   0        0        0      202 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/any_scale/src/__init__.py
--rw-r--r--   0        0        0     2054 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/any_scale/src/anyscale.py
--rw-r--r--   0        0        0     1327 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/any_scale/src/static/json_schema.json
--rw-r--r--   0        0        0       37 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/azure_open_ai/README.md
--rw-r--r--   0        0        0      482 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/azure_open_ai/pyproject.toml
--rw-r--r--   0        0        0      219 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/azure_open_ai/src/__init__.py
--rw-r--r--   0        0        0     2290 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py
--rw-r--r--   0        0        0     1681 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0       69 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/constants.py
--rw-r--r--   0        0        0      850 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/helper.py
--rw-r--r--   0        0        0     1573 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/llm_adapter.py
--rw-r--r--   0        0        0       34 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/mistral/README.md
--rw-r--r--   0        0        0      473 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/mistral/pyproject.toml
--rw-r--r--   0        0        0      197 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/mistral/src/__init__.py
--rw-r--r--   0        0        0     1774 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/mistral/src/mistral.py
--rw-r--r--   0        0        0      852 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/mistral/src/static/json_schema.json
--rw-r--r--   0        0        0       31 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/open_ai/README.md
--rw-r--r--   0        0        0      470 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/open_ai/pyproject.toml
--rw-r--r--   0        0        0      193 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/open_ai/src/__init__.py
--rw-r--r--   0        0        0     2240 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/open_ai/src/open_ai.py
--rw-r--r--   0        0        0     1489 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0       26 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/palm/README.md
--rw-r--r--   0        0        0      462 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/palm/pyproject.toml
--rw-r--r--   0        0        0      182 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/palm/src/__init__.py
--rw-r--r--   0        0        0     1871 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/palm/src/palm.py
--rw-r--r--   0        0        0      989 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/palm/src/static/json_schema.json
--rw-r--r--   0        0        0     1963 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/register.py
--rw-r--r--   0        0        0       33 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/replicate/README.md
--rw-r--r--   0        0        0      474 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/replicate/pyproject.toml
--rw-r--r--   0        0        0      207 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/replicate/src/__init__.py
--rw-r--r--   0        0        0     1714 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/replicate/src/replicate.py
--rw-r--r--   0        0        0      840 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/replicate/src/static/json_schema.json
--rw-r--r--   0        0        0      273 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/vertex_ai/README.md
--rw-r--r--   0        0        0      444 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/vertex_ai/pyproject.toml
--rw-r--r--   0        0        0      203 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/vertex_ai/src/__init__.py
--rw-r--r--   0        0        0      964 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json
--rw-r--r--   0        0        0     2085 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py
--rw-r--r--   0        0        0      165 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/__init__.py
--rw-r--r--   0        0        0      430 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/constants.py
--rw-r--r--   0        0        0       42 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/README.md
--rw-r--r--   0        0        0      491 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/src/README.md
--rw-r--r--   0        0        0      237 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/src/__init__.py
--rw-r--r--   0        0        0     5955 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py
--rw-r--r--   0        0        0      817 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json
--rw-r--r--   0        0        0      978 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/ocr_adapter.py
--rw-r--r--   0        0        0     1964 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/register.py
--rw-r--r--   0        0        0      277 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/registry.py
--rw-r--r--   0        0        0     1745 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/utils.py
--rw-r--r--   0        0        0      181 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/__init__.py
--rw-r--r--   0        0        0      225 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/constants.py
--rw-r--r--   0        0        0     4289 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/helper.py
--rw-r--r--   0        0        0       27 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/milvus/README.md
--rw-r--r--   0        0        0      485 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/milvus/pyproject.toml
--rw-r--r--   0        0        0      188 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/milvus/src/__init__.py
--rw-r--r--   0        0        0     2795 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/milvus/src/milvus.py
--rw-r--r--   0        0        0      805 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json
--rw-r--r--   0        0        0       29 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/pinecone/README.md
--rw-r--r--   0        0        0      489 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/pinecone/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/pinecone/src/__init__.py
--rw-r--r--   0        0        0     3732 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/pinecone/src/pinecone.py
--rw-r--r--   0        0        0      771 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json
--rw-r--r--   0        0        0       29 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/postgres/README.md
--rw-r--r--   0        0        0      489 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/postgres/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/postgres/src/__init__.py
--rw-r--r--   0        0        0     3923 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/postgres/src/postgres.py
--rw-r--r--   0        0        0      912 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json
--rw-r--r--   0        0        0       27 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/qdrant/README.md
--rw-r--r--   0        0        0      485 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/qdrant/pyproject.toml
--rw-r--r--   0        0        0      188 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/qdrant/src/__init__.py
--rw-r--r--   0        0        0     2719 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/qdrant/src/qdrant.py
--rw-r--r--   0        0        0      571 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json
--rw-r--r--   0        0        0     2039 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/register.py
--rw-r--r--   0        0        0    75042 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/samples/sample1.txt
--rw-r--r--   0        0        0       30 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/supabase/README.md
--rw-r--r--   0        0        0      489 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/supabase/pyproject.toml
--rw-r--r--   0        0        0      199 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/supabase/src/__init__.py
--rw-r--r--   0        0        0      937 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json
--rw-r--r--   0        0        0     3371 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/supabase/src/supabase.py
--rw-r--r--   0        0        0     1328 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/vectordb_adapter.py
--rw-r--r--   0        0        0       29 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/weaviate/README.md
--rw-r--r--   0        0        0      489 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/weaviate/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/weaviate/src/__init__.py
--rw-r--r--   0        0        0      678 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json
--rw-r--r--   0        0        0     3715 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/weaviate/src/weaviate.py
--rw-r--r--   0        0        0      174 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/__init__.py
--rw-r--r--   0        0        0      145 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/constants.py
--rw-r--r--   0        0        0     5407 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/helper.py
--rw-r--r--   0        0        0       40 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/README.md
--rw-r--r--   0        0        0      495 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/pyproject.toml
--rw-r--r--   0        0        0      217 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/src/__init__.py
--rw-r--r--   0        0        0      981 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/src/constants.py
--rw-r--r--   0        0        0     6559 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py
--rw-r--r--   0        0        0     3115 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json
--rw-r--r--   0        0        0     1991 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/register.py
--rw-r--r--   0        0        0       51 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_community/README.md
--rw-r--r--   0        0        0      499 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_community/pyproject.toml
--rw-r--r--   0        0        0      255 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_community/src/__init__.py
--rw-r--r--   0        0        0      583 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json
--rw-r--r--   0        0        0     1460 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py
--rw-r--r--   0        0        0       52 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_enterprise/README.md
--rw-r--r--   0        0        0      499 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_enterprise/pyproject.toml
--rw-r--r--   0        0        0      259 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_enterprise/src/__init__.py
--rw-r--r--   0        0        0      805 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json
--rw-r--r--   0        0        0     1465 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py
--rw-r--r--   0        0        0     1006 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/x2text_adapter.py
--rw-r--r--   0        0        0     2673 1970-01-01 00:00:00.000000 unstract_adapters-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-16 05:28:49.521915 unstract_adapters-0.9.1/LICENSE
+-rw-r--r--   0        0        0      915 2024-04-16 05:28:49.521915 unstract_adapters-0.9.1/README.md
+-rw-r--r--   0        0        0     2632 2024-04-16 05:29:10.113827 unstract_adapters-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      298 2024-04-16 05:28:49.521915 unstract_adapters-0.9.1/src/unstract/adapters/__init__.py
+-rw-r--r--   0        0        0     2805 2024-04-16 05:28:49.521915 unstract_adapters-0.9.1/src/unstract/adapters/adapterkit.py
+-rw-r--r--   0        0        0     1830 2024-04-16 05:28:49.521915 unstract_adapters-0.9.1/src/unstract/adapters/base.py
+-rw-r--r--   0        0        0      282 2024-04-16 05:28:49.521915 unstract_adapters-0.9.1/src/unstract/adapters/constants.py
+-rw-r--r--   0        0        0      183 2024-04-16 05:28:49.521915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-16 05:28:49.521915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/azure_open_ai/README.md
+-rw-r--r--   0        0        0      494 2024-04-16 05:28:49.521915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/azure_open_ai/pyproject.toml
+-rw-r--r--   0        0        0      216 2024-04-16 05:28:49.521915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/azure_open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2468 2024-04-16 05:28:49.521915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py
+-rw-r--r--   0        0        0     1548 2024-04-16 05:28:49.521915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0     1145 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/embedding_adapter.py
+-rw-r--r--   0        0        0     1319 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/helper.py
+-rw-r--r--   0        0        0       42 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/hugging_face/README.md
+-rw-r--r--   0        0        0      491 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/hugging_face/pyproject.toml
+-rw-r--r--   0        0        0      216 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/hugging_face/src/__init__.py
+-rw-r--r--   0        0        0     2449 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py
+-rw-r--r--   0        0        0      940 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json
+-rw-r--r--   0        0        0       30 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/open_ai/README.md
+-rw-r--r--   0        0        0      482 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/open_ai/pyproject.toml
+-rw-r--r--   0        0        0      190 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2055 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/open_ai/src/open_ai.py
+-rw-r--r--   0        0        0      719 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0       35 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/palm/README.md
+-rw-r--r--   0        0        0      476 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/palm/pyproject.toml
+-rw-r--r--   0        0        0      179 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/palm/src/__init__.py
+-rw-r--r--   0        0        0     1993 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/palm/src/palm.py
+-rw-r--r--   0        0        0      804 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/palm/src/static/json_schema.json
+-rw-r--r--   0        0        0       46 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/qdrant_fast_embed/README.md
+-rw-r--r--   0        0        0      500 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/qdrant_fast_embed/pyproject.toml
+-rw-r--r--   0        0        0      240 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/__init__.py
+-rw-r--r--   0        0        0     1784 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py
+-rw-r--r--   0        0        0      553 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json
+-rw-r--r--   0        0        0     2086 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/embedding/register.py
+-rw-r--r--   0        0        0      184 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/enums.py
+-rw-r--r--   0        0        0      502 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/exceptions.py
+-rw-r--r--   0        0        0      165 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/anthropic/README.md
+-rw-r--r--   0        0        0      474 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/anthropic/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/anthropic/src/__init__.py
+-rw-r--r--   0        0        0     2000 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/anthropic/src/anthropic.py
+-rw-r--r--   0        0        0     1017 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/anthropic/src/static/json_schema.json
+-rw-r--r--   0        0        0       33 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/any_scale/README.md
+-rw-r--r--   0        0        0      473 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/any_scale/pyproject.toml
+-rw-r--r--   0        0        0      202 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/any_scale/src/__init__.py
+-rw-r--r--   0        0        0     2054 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/any_scale/src/anyscale.py
+-rw-r--r--   0        0        0     1327 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/any_scale/src/static/json_schema.json
+-rw-r--r--   0        0        0       37 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/azure_open_ai/README.md
+-rw-r--r--   0        0        0      482 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/azure_open_ai/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/azure_open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2290 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py
+-rw-r--r--   0        0        0     1681 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0       69 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/constants.py
+-rw-r--r--   0        0        0      850 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/helper.py
+-rw-r--r--   0        0        0     1573 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/llm_adapter.py
+-rw-r--r--   0        0        0       34 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/mistral/README.md
+-rw-r--r--   0        0        0      473 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/mistral/pyproject.toml
+-rw-r--r--   0        0        0      197 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/mistral/src/__init__.py
+-rw-r--r--   0        0        0     1774 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/mistral/src/mistral.py
+-rw-r--r--   0        0        0      852 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/mistral/src/static/json_schema.json
+-rw-r--r--   0        0        0       31 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/open_ai/README.md
+-rw-r--r--   0        0        0      470 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/open_ai/pyproject.toml
+-rw-r--r--   0        0        0      193 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2240 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/open_ai/src/open_ai.py
+-rw-r--r--   0        0        0     1489 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0       26 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/palm/README.md
+-rw-r--r--   0        0        0      462 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/palm/pyproject.toml
+-rw-r--r--   0        0        0      182 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/palm/src/__init__.py
+-rw-r--r--   0        0        0     1871 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/palm/src/palm.py
+-rw-r--r--   0        0        0      989 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/palm/src/static/json_schema.json
+-rw-r--r--   0        0        0     1963 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/register.py
+-rw-r--r--   0        0        0       33 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/replicate/README.md
+-rw-r--r--   0        0        0      474 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/replicate/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/replicate/src/__init__.py
+-rw-r--r--   0        0        0     1714 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/replicate/src/replicate.py
+-rw-r--r--   0        0        0      840 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/replicate/src/static/json_schema.json
+-rw-r--r--   0        0        0      273 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/vertex_ai/README.md
+-rw-r--r--   0        0        0      444 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/vertex_ai/pyproject.toml
+-rw-r--r--   0        0        0      203 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/vertex_ai/src/__init__.py
+-rw-r--r--   0        0        0      964 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0     2085 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py
+-rw-r--r--   0        0        0      165 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/ocr/__init__.py
+-rw-r--r--   0        0        0      430 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/ocr/constants.py
+-rw-r--r--   0        0        0       42 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/ocr/google_document_ai/README.md
+-rw-r--r--   0        0        0      491 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/ocr/google_document_ai/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/ocr/google_document_ai/src/README.md
+-rw-r--r--   0        0        0      237 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/ocr/google_document_ai/src/__init__.py
+-rw-r--r--   0        0        0     5955 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py
+-rw-r--r--   0        0        0      817 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0      978 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/ocr/ocr_adapter.py
+-rw-r--r--   0        0        0     1964 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/ocr/register.py
+-rw-r--r--   0        0        0      277 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/registry.py
+-rw-r--r--   0        0        0     1745 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/utils.py
+-rw-r--r--   0        0        0      181 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/constants.py
+-rw-r--r--   0        0        0     4289 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/helper.py
+-rw-r--r--   0        0        0       27 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/milvus/README.md
+-rw-r--r--   0        0        0      485 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/milvus/pyproject.toml
+-rw-r--r--   0        0        0      188 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/milvus/src/__init__.py
+-rw-r--r--   0        0        0     2795 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/milvus/src/milvus.py
+-rw-r--r--   0        0        0      805 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json
+-rw-r--r--   0        0        0       29 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/pinecone/README.md
+-rw-r--r--   0        0        0      489 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/pinecone/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/pinecone/src/__init__.py
+-rw-r--r--   0        0        0     3732 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/pinecone/src/pinecone.py
+-rw-r--r--   0        0        0      771 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json
+-rw-r--r--   0        0        0       29 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/postgres/README.md
+-rw-r--r--   0        0        0      489 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/postgres/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/postgres/src/__init__.py
+-rw-r--r--   0        0        0     3923 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/postgres/src/postgres.py
+-rw-r--r--   0        0        0      912 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json
+-rw-r--r--   0        0        0       27 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/qdrant/README.md
+-rw-r--r--   0        0        0      485 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/qdrant/pyproject.toml
+-rw-r--r--   0        0        0      188 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/qdrant/src/__init__.py
+-rw-r--r--   0        0        0     2719 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/qdrant/src/qdrant.py
+-rw-r--r--   0        0        0      571 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json
+-rw-r--r--   0        0        0     2039 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/register.py
+-rw-r--r--   0        0        0    75042 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/samples/sample1.txt
+-rw-r--r--   0        0        0       30 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/supabase/README.md
+-rw-r--r--   0        0        0      489 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/supabase/pyproject.toml
+-rw-r--r--   0        0        0      199 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/supabase/src/__init__.py
+-rw-r--r--   0        0        0      937 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json
+-rw-r--r--   0        0        0     3371 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/supabase/src/supabase.py
+-rw-r--r--   0        0        0     1328 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/vectordb_adapter.py
+-rw-r--r--   0        0        0       29 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/weaviate/README.md
+-rw-r--r--   0        0        0      489 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/weaviate/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/weaviate/src/__init__.py
+-rw-r--r--   0        0        0      678 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json
+-rw-r--r--   0        0        0     3715 2024-04-16 05:28:49.525915 unstract_adapters-0.9.1/src/unstract/adapters/vectordb/weaviate/src/weaviate.py
+-rw-r--r--   0        0        0      174 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/constants.py
+-rw-r--r--   0        0        0     5407 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/helper.py
+-rw-r--r--   0        0        0       40 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/llm_whisperer/README.md
+-rw-r--r--   0        0        0      495 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/llm_whisperer/pyproject.toml
+-rw-r--r--   0        0        0      217 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/llm_whisperer/src/__init__.py
+-rw-r--r--   0        0        0      981 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/llm_whisperer/src/constants.py
+-rw-r--r--   0        0        0     6559 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py
+-rw-r--r--   0        0        0     3115 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json
+-rw-r--r--   0        0        0     1991 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/register.py
+-rw-r--r--   0        0        0       51 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/unstructured_community/README.md
+-rw-r--r--   0        0        0      499 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/unstructured_community/pyproject.toml
+-rw-r--r--   0        0        0      255 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/unstructured_community/src/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json
+-rw-r--r--   0        0        0     1460 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py
+-rw-r--r--   0        0        0       52 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/unstructured_enterprise/README.md
+-rw-r--r--   0        0        0      499 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/unstructured_enterprise/pyproject.toml
+-rw-r--r--   0        0        0      259 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/unstructured_enterprise/src/__init__.py
+-rw-r--r--   0        0        0      805 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json
+-rw-r--r--   0        0        0     1465 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py
+-rw-r--r--   0        0        0     1006 2024-04-16 05:28:49.529915 unstract_adapters-0.9.1/src/unstract/adapters/x2text/x2text_adapter.py
+-rw-r--r--   0        0        0     2741 1970-01-01 00:00:00.000000 unstract_adapters-0.9.1/PKG-INFO
```

### Comparing `unstract_adapters-0.9.0/LICENSE` & `unstract_adapters-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/README.md` & `unstract_adapters-0.9.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div align="center">
-<img src="docs/assets/unstract_u_logo.png" style="height: 120px">
+<img src="https://raw.githubusercontent.com/Zipstack/unstract-adapters/main/docs/assets/unstract_u_logo.png" style="height: 120px">
 
 # Unstract
 
 ## No-code LLM Platform to launch APIs and ETL Pipelines to structure unstructured documents
 
 </div>
```

### Comparing `unstract_adapters-0.9.0/pyproject.toml` & `unstract_adapters-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-version = "0.9.0"
+version = "0.9.1"
 
 [project.urls]
 Homepage = "https://unstract.com"
 "Release notes" = "https://github.com/Zipstack/unstract-adapters/releases"
 Source = "https://github.com/Zipstack/unstract-adapters"
 
 [project.license]
```

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/adapterkit.py` & `unstract_adapters-0.9.1/src/unstract/adapters/adapterkit.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/base.py` & `unstract_adapters-0.9.1/src/unstract/adapters/base.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py` & `unstract_adapters-0.9.1/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/embedding/embedding_adapter.py` & `unstract_adapters-0.9.1/src/unstract/adapters/embedding/embedding_adapter.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/embedding/helper.py` & `unstract_adapters-0.9.1/src/unstract/adapters/embedding/helper.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py` & `unstract_adapters-0.9.1/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/embedding/open_ai/src/open_ai.py` & `unstract_adapters-0.9.1/src/unstract/adapters/embedding/open_ai/src/open_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/embedding/palm/src/palm.py` & `unstract_adapters-0.9.1/src/unstract/adapters/embedding/palm/src/palm.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/embedding/palm/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/embedding/palm/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py` & `unstract_adapters-0.9.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/embedding/register.py` & `unstract_adapters-0.9.1/src/unstract/adapters/embedding/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/anthropic/src/anthropic.py` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/anthropic/src/anthropic.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/anthropic/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/anthropic/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/any_scale/src/anyscale.py` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/any_scale/src/anyscale.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/any_scale/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/any_scale/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/helper.py` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/helper.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/llm_adapter.py` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/llm_adapter.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/mistral/src/mistral.py` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/mistral/src/mistral.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/mistral/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/mistral/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/open_ai/src/open_ai.py` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/open_ai/src/open_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/open_ai/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/palm/src/palm.py` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/palm/src/palm.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/palm/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/palm/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/register.py` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/replicate/src/replicate.py` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/replicate/src/replicate.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/replicate/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/replicate/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py` & `unstract_adapters-0.9.1/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py` & `unstract_adapters-0.9.1/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/ocr/ocr_adapter.py` & `unstract_adapters-0.9.1/src/unstract/adapters/ocr/ocr_adapter.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/ocr/register.py` & `unstract_adapters-0.9.1/src/unstract/adapters/ocr/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/utils.py` & `unstract_adapters-0.9.1/src/unstract/adapters/utils.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/helper.py` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/helper.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/milvus/src/milvus.py` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/milvus/src/milvus.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/pinecone/src/pinecone.py` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/pinecone/src/pinecone.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/postgres/src/postgres.py` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/postgres/src/postgres.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/qdrant/src/qdrant.py` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/qdrant/src/qdrant.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/register.py` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/samples/sample1.txt` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/samples/sample1.txt`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/supabase/src/supabase.py` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/supabase/src/supabase.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/vectordb_adapter.py` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/vectordb_adapter.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/weaviate/src/weaviate.py` & `unstract_adapters-0.9.1/src/unstract/adapters/vectordb/weaviate/src/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/x2text/helper.py` & `unstract_adapters-0.9.1/src/unstract/adapters/x2text/helper.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/src/constants.py` & `unstract_adapters-0.9.1/src/unstract/adapters/x2text/llm_whisperer/src/constants.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py` & `unstract_adapters-0.9.1/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/x2text/register.py` & `unstract_adapters-0.9.1/src/unstract/adapters/x2text/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py` & `unstract_adapters-0.9.1/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json` & `unstract_adapters-0.9.1/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py` & `unstract_adapters-0.9.1/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/src/unstract/adapters/x2text/x2text_adapter.py` & `unstract_adapters-0.9.1/src/unstract/adapters/x2text/x2text_adapter.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.9.0/PKG-INFO` & `unstract_adapters-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: unstract-adapters
-Version: 0.9.0
+Version: 0.9.1
 Summary: Unstract interface for LLMs, Embeddings and VectorDBs
-Author-Email: Zipstack Inc. <devsupport@zipstack.com>
+Author-Email: "Zipstack Inc." <devsupport@zipstack.com>
 License: AGPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
@@ -34,15 +34,15 @@
 Requires-Dist: llama-index-llms-vertex==0.1.5
 Requires-Dist: llama-index-llms-replicate==0.1.3
 Requires-Dist: filetype~=1.2.0
 Requires-Dist: singleton-decorator~=1.0.0
 Description-Content-Type: text/markdown
 
 <div align="center">
-<img src="docs/assets/unstract_u_logo.png" style="height: 120px">
+<img src="https://raw.githubusercontent.com/Zipstack/unstract-adapters/main/docs/assets/unstract_u_logo.png" style="height: 120px">
 
 # Unstract
 
 ## No-code LLM Platform to launch APIs and ETL Pipelines to structure unstructured documents
 
 </div>
```

