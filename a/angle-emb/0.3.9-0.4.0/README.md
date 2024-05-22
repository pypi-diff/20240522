# Comparing `tmp/angle_emb-0.3.9.tar.gz` & `tmp/angle_emb-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angle_emb-0.3.9.tar", last modified: Thu Mar 14 02:57:26 2024, max compression
+gzip compressed data, was "angle_emb-0.4.0.tar", last modified: Tue May 21 09:23:20 2024, max compression
```

## Comparing `angle_emb-0.3.9.tar` & `angle_emb-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-03-14 02:57:26.923995 angle_emb-0.3.9/
--rw-r--r--   0 seanlee    (501) staff       (20)     1061 2024-03-14 02:21:04.000000 angle_emb-0.3.9/LICENSE
--rw-r--r--   0 seanlee    (501) staff       (20)    15284 2024-03-14 02:57:26.924222 angle_emb-0.3.9/PKG-INFO
--rw-r--r--   0 seanlee    (501) staff       (20)    14568 2024-03-14 02:21:04.000000 angle_emb-0.3.9/README.md
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-03-14 02:57:26.920503 angle_emb-0.3.9/angle_emb/
--rw-r--r--   0 seanlee    (501) staff       (20)       70 2024-03-14 02:57:04.000000 angle_emb-0.3.9/angle_emb/__init__.py
--rw-r--r--   0 seanlee    (501) staff       (20)    65297 2024-03-14 02:56:57.000000 angle_emb-0.3.9/angle_emb/angle.py
--rw-r--r--   0 seanlee    (501) staff       (20)    11029 2024-03-14 02:56:57.000000 angle_emb-0.3.9/angle_emb/train_cli.py
--rw-r--r--   0 seanlee    (501) staff       (20)      118 2024-03-14 02:21:04.000000 angle_emb-0.3.9/angle_emb/utils.py
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-03-14 02:57:26.923667 angle_emb-0.3.9/angle_emb.egg-info/
--rw-r--r--   0 seanlee    (501) staff       (20)    15284 2024-03-14 02:57:26.000000 angle_emb-0.3.9/angle_emb.egg-info/PKG-INFO
--rw-r--r--   0 seanlee    (501) staff       (20)      351 2024-03-14 02:57:26.000000 angle_emb-0.3.9/angle_emb.egg-info/SOURCES.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-03-14 02:57:26.000000 angle_emb-0.3.9/angle_emb.egg-info/dependency_links.txt
--rw-r--r--   0 seanlee    (501) staff       (20)       59 2024-03-14 02:57:26.000000 angle_emb-0.3.9/angle_emb.egg-info/entry_points.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-03-14 02:57:26.000000 angle_emb-0.3.9/angle_emb.egg-info/not-zip-safe
--rw-r--r--   0 seanlee    (501) staff       (20)       87 2024-03-14 02:57:26.000000 angle_emb-0.3.9/angle_emb.egg-info/requires.txt
--rw-r--r--   0 seanlee    (501) staff       (20)       10 2024-03-14 02:57:26.000000 angle_emb-0.3.9/angle_emb.egg-info/top_level.txt
--rw-r--r--   0 seanlee    (501) staff       (20)      202 2024-03-14 02:57:26.924786 angle_emb-0.3.9/setup.cfg
--rw-r--r--   0 seanlee    (501) staff       (20)     1525 2024-03-14 02:57:04.000000 angle_emb-0.3.9/setup.py
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-21 09:23:20.053603 angle_emb-0.4.0/
+-rw-r--r--   0 seanlee    (501) staff       (20)     1061 2024-01-15 11:58:12.000000 angle_emb-0.4.0/LICENSE
+-rw-r--r--   0 seanlee    (501) staff       (20)    14916 2024-05-21 09:23:20.053914 angle_emb-0.4.0/PKG-INFO
+-rw-r--r--   0 seanlee    (501) staff       (20)    14199 2024-05-21 09:17:37.000000 angle_emb-0.4.0/README.md
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-21 09:23:20.043697 angle_emb-0.4.0/angle_emb/
+-rw-r--r--   0 seanlee    (501) staff       (20)       70 2024-05-21 09:22:51.000000 angle_emb-0.4.0/angle_emb/__init__.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    70346 2024-05-21 09:01:40.000000 angle_emb-0.4.0/angle_emb/angle.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    13589 2024-05-21 09:01:40.000000 angle_emb-0.4.0/angle_emb/angle_trainer.py
+-rw-r--r--   0 seanlee    (501) staff       (20)      512 2024-05-21 09:01:40.000000 angle_emb-0.4.0/angle_emb/utils.py
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-21 09:23:20.053133 angle_emb-0.4.0/angle_emb.egg-info/
+-rw-r--r--   0 seanlee    (501) staff       (20)    14916 2024-05-21 09:23:19.000000 angle_emb-0.4.0/angle_emb.egg-info/PKG-INFO
+-rw-r--r--   0 seanlee    (501) staff       (20)      355 2024-05-21 09:23:19.000000 angle_emb-0.4.0/angle_emb.egg-info/SOURCES.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-05-21 09:23:19.000000 angle_emb-0.4.0/angle_emb.egg-info/dependency_links.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)       63 2024-05-21 09:23:19.000000 angle_emb-0.4.0/angle_emb.egg-info/entry_points.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-01-15 12:03:51.000000 angle_emb-0.4.0/angle_emb.egg-info/not-zip-safe
+-rw-r--r--   0 seanlee    (501) staff       (20)       87 2024-05-21 09:23:19.000000 angle_emb-0.4.0/angle_emb.egg-info/requires.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)       10 2024-05-21 09:23:19.000000 angle_emb-0.4.0/angle_emb.egg-info/top_level.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)      202 2024-05-21 09:23:20.113137 angle_emb-0.4.0/setup.cfg
+-rw-r--r--   0 seanlee    (501) staff       (20)     1529 2024-05-21 09:22:51.000000 angle_emb-0.4.0/setup.py
```

### Comparing `angle_emb-0.3.9/LICENSE` & `angle_emb-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `angle_emb-0.3.9/PKG-INFO` & `angle_emb-0.4.0/angle_emb.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: angle_emb
-Version: 0.3.9
+Name: angle-emb
+Version: 0.4.0
 Summary: AnglE-optimize Text Embeddings
 Author: sean lee
 Author-email: xmlee97@gmail.com
 Keywords: angle_emb
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -16,253 +16,221 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <small>EN | [简体中文](README_zh.md) </small>
 
-# [AnglE📐: Angle-optimized Text Embeddings](https://arxiv.org/abs/2309.12871)
+# AnglE📐
 
 > It is Angle 📐, not Angel 👼.
 
-🔥 **A New SOTA** for Semantic Textual Similarity! 
-
-
-🔥 **Our universal sentence embedding [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) achieves SOTA on the [MTEB Leaderboard](https://huggingface.co/spaces/mteb/leaderboard) with an average score of 64.64!**
-
+📘 document: https://angle.readthedocs.io/en/latest/index.html
 
 <a href="https://arxiv.org/abs/2309.12871">
-    <img src="https://img.shields.io/badge/Arxiv-2306.06843-yellow.svg?style=flat-square" alt="https://arxiv.org/abs/2309.12871" />
+    <img src="https://img.shields.io/badge/Arxiv-2309.12871-yellow.svg?style=flat-square" alt="https://arxiv.org/abs/2309.12871" />
 </a>
 <a href="https://pypi.org/project/angle_emb/">
     <img src="https://img.shields.io/pypi/v/angle_emb?style=flat-square" alt="PyPI version" />
 </a>
 <a href="https://pypi.org/project/angle_emb/">
     <img src="https://img.shields.io/pypi/dm/angle_emb?style=flat-square" alt="PyPI Downloads" />
 </a>
-<a href="http://makeapullrequest.com">
-    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="http://makeapullrequest.com" />
+<a href="https://angle.readthedocs.io/en/latest/index.html">
+    <img src="https://readthedocs.org/projects/angle/badge/?version=latest&style=flat-square" alt="Read the docs" />
 </a>
 
+
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sick-r-1)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sick-r-1?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts16)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts16?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts15)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts15?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts14)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts14?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts13)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts13?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts12)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts12?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts-benchmark)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts-benchmark?p=angle-optimized-text-embeddings)
 
+📢 **Train/Infer Powerful Sentence Embeddings with AnglE.**
+This library is from the paper: [AnglE: Angle-optimized Text Embeddings](https://arxiv.org/abs/2309.12871). It allows for training state-of-the-art BERT/LLM-based sentence embeddings with just a few lines of code. AnglE is also a general sentence embedding inference framework, allowing for infering a variety of transformer-based sentence embeddings.
 
-<details>
-<summary>📊 Results on MTEB Leaderboard [click to expand]</summary>
-<p align='center'>
-<img src='assets/UAE-MTEB.png'>
-</p>
-</details>
-
-<details>
-<summary>📊 Results on STS benchmark [click to expand]</summary>
-<p align='center'>
-<img src='assets/angle-results.png'>
-</p>
-</details>
-
-## 🤗 Pretrained Models
-| 🤗 HF | LoRA Weight | Dependent Backbone | LLM | Language | Prompt | Pooling Strategy | Examples |
-|----|------|------|------|------|------|------|------|
-| [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) |  N | N | N | EN | `Prompts.C` for retrieval purposes, `None` for others | cls | [![Seach Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WOYD6f8gb_wpkUm_57K8pEDgjlGJd6oB?usp=drive_link) |
-| [SeanLee97/angle-llama-13b-nli](https://huggingface.co/SeanLee97/angle-llama-13b-nli) | Y |  NousResearch/Llama-2-13b-hf | Y | EN | `Prompts.A` | last token | / | 
-| [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-7b-nli-v2) | Y |  NousResearch/Llama-2-7b-hf | Y | EN | `Prompts.A` | last token | / |
-| [SeanLee97/angle-llama-7b-nli-20231027](https://huggingface.co/SeanLee97/angle-llama-7b-nli-20231027) | Y |  NousResearch/Llama-2-7b-hf | Y | EN | `Prompts.A` | last token | / |
-| [SeanLee97/angle-bert-base-uncased-nli-en-v1](https://huggingface.co/SeanLee97/angle-bert-base-uncased-nli-en-v1) | N |  N | N | EN | N | `cls_avg` | / |
-| [SeanLee97/angle-roberta-wwm-base-zhnli-v1](https://huggingface.co/SeanLee97/angle-roberta-wwm-base-zhnli-v1) | N |  N | N | ZH-CN | N | `cls` | / |
-| [SeanLee97/angle-llama-7b-zhnli-v1](https://huggingface.co/SeanLee97/angle-llama-7b-zhnli-v1) | Y |  NousResearch/Llama-2-7b-hf | Y | ZH-CN | `Prompts.B` | last token | / |
- 
-💡 If the selected model is a LoRA weight, it must specify the corresponding dependent backbone.
-
-For our STS Experiment, please refer to https://github.com/SeanLee97/AnglE/tree/main/examples/NLI
-
-</details>
-
-## Results
-
-### English STS Results
-
-| Model | STS12 | STS13 | STS14 | STS15 | STS16 | STSBenchmark | SICKRelatedness |  Avg. |
-| ------- |-------|-------|-------|-------|-------|--------------|-----------------|-------|
-| [SeanLee97/angle-llama-7b-nli-20231027](https://huggingface.co/SeanLee97/angle-llama-7b-nli-20231027) | 78.68 | 90.58 | 85.49 | 89.56 | 86.91 |    88.92     |      81.18      | 85.90 |
-| [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-7b-nli-v2) | 79.00 | 90.56 | 85.79 | 89.43 | 87.00 |    88.97     |      80.94      | 85.96 |
-| [SeanLee97/angle-llama-13b-nli](https://huggingface.co/SeanLee97/angle-llama-13b-nli)  | 79.33 | 90.65 | 86.89 | 90.45 | 87.32 |    89.69     |      81.32       | **86.52** |
-| [SeanLee97/angle-bert-base-uncased-nli-en-v1](https://huggingface.co/SeanLee97/angle-bert-base-uncased-nli-en-v1) | 75.09 | 85.56 | 80.66 | 86.44 | 82.47 | 85.16 | 81.23 | 82.37 |
-
-
-### Chinese STS Results
-
-| Model | ATEC | BQ	| LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc | Avg. |
-| ------- |-------|-------|-------|-------|-------|--------------|-----------------|-------|
-| ^[shibing624/text2vec-bge-large-chinese](https://huggingface.co/shibing624/text2vec-bge-large-chinese) | 38.41 | 61.34 | 71.72 | 35.15 | 76.44 | 71.81 | 63.15 | 59.72 |
-| ^[shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase) |	44.89 | 63.58 | 74.24 | 40.90 | 78.93 | 76.70 | 63.30 | 63.08 |
-| [SeanLee97/angle-roberta-wwm-base-zhnli-v1](https://huggingface.co/SeanLee97/angle-roberta-wwm-base-zhnli-v1) | 49.49 | 72.47 | 78.33 | 59.13 | 77.14 |    72.36     |      60.53      | **67.06** |
-| [SeanLee97/angle-llama-7b-zhnli-v1](https://huggingface.co/SeanLee97/angle-llama-7b-zhnli-v1) | 50.44 | 71.95 | 78.90 | 56.57 | 81.11 | 68.11 | 52.02 | 65.59 |
+## ✨ Features
 
-^ denotes baselines, their results are retrieved from: https://github.com/shibing624/text2vec
+**Loss**:
+- 📐 AnglE loss
+- ⚖ Contrastive loss
+- 📏 CoSENT loss
+- ☕️ Espresso loss (previously known as 2DMSE, detail: [README_ESE](README_ESE.md))
 
+**Backbones**:
+- BERT-based models (BERT, RoBERTa, ELECTRA, ALBERT, etc.)
+- LLM-based models (LLaMA, Mistral, Qwen, etc.)
+- Bi-directional LLM-based models (LLaMA, Mistral, Qwen, OpenELMo, etc.. refer to: https://github.com/WhereIsAI/BiLLM)
 
-## Usage
+**Training**:
+- Single-GPU training
+- Multi-GPU training
 
-AnglE supports two APIs, one is the `transformers` API, the other is the `AnglE` API. If you want to use the `AnglE` API, please install AnglE first:
 
-```bash
-python -m pip install -U angle-emb
-```
+> <a href="http://makeapullrequest.com"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="http://makeapullrequest.com" /></a> 
+    More features will be added in the future. 
 
-### UAE
+## 🏆 Achievements
 
-1) For Retrieval Purposes
+📅  May 16, 2024 | Paper "[AnglE: Angle-optimized Text Embeddings](https://arxiv.org/abs/2309.12871)" is accepted by ACL 2024 Main Conference.
 
-For retrieval purposes, please use the prompt `Prompts.C`.
+📅  Mar 13, 2024 | Paper "[BeLLM: Backward Dependency Enhanced Large Language Model for Sentence Embeddings](https://arxiv.org/abs/2311.05296)" is accepted by NAACL 2024 Main Conference.
 
-```python
-from angle_emb import AnglE, Prompts
 
-angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1', pooling_strategy='cls').cuda()
-angle.set_prompt(prompt=Prompts.C)
-vec = angle.encode({'text': 'hello world'}, to_numpy=True)
-print(vec)
-vecs = angle.encode([{'text': 'hello world1'}, {'text': 'hello world2'}], to_numpy=True)
-print(vecs)
-```
+📅  Mar 8, 2024 | 🍞 [mixedbread's embedding](https://www.mixedbread.ai/blog/mxbai-embed-large-v1) ([mixedbread-ai/mxbai-embed-large-v1](https://huggingface.co/mixedbread-ai/mxbai-embed-large-v1)) achieves SOTA on the [MTEB Leaderboard](https://huggingface.co/spaces/mteb/leaderboard) with an average score of **64.68**! The model is trained using AnglE. Congrats mixedbread!
 
-2) For non-Retrieval Purposes
 
-```python
-from angle_emb import AnglE
+📅  Dec 4, 2023 | Our universal sentence embedding [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) achieves SOTA on the [MTEB Leaderboard](https://huggingface.co/spaces/mteb/leaderboard) with an average score of **64.64**! The model is trained using AnglE.
+
+
+📅 Dec, 2023 | AnglE achieves SOTA performance on the STS Bechmark Semantic Textual Similarity! 
 
-angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1', pooling_strategy='cls').cuda()
-vec = angle.encode('hello world', to_numpy=True)
-print(vec)
-vecs = angle.encode(['hello world1', 'hello world2'], to_numpy=True)
-print(vecs)
-```
 
-<details>
-<summary>Difference between retrieval and non-retrieval sentence embeddings. [click to expand]</summary>
+## 🤗 Official Pretrained Models
 
-In UAE, we use different approaches for retrieval and non-retrieval tasks, each serving a different purpose. 
+BERT-based models:
 
-**Retrieval tasks aim to find relevant documents, and as a result, the related documents may not have strict semantic similarities to each other.**
+|  🤗 HF | Max Tokens | Pooling Strategy | Scenario |
+|----|------|------|------|
+| [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) | 512 | cls | English, General-purpose |
+| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) |  512 | cls | Code Similarity |
 
-For instance, when querying "How about ChatGPT?", the related documents are those that contain information related to "ChatGPT," such as "ChatGPT is amazing..." or "ChatGPT is bad....".
+LLM-based models:
 
-Conversely, **non-retrieval tasks, such as semantic textual similarity, require sentences that are semantically similar.**
+| 🤗 HF (lora weight) | Backbone | Max Tokens | Prompts |  Pooling Strategy | Scenario  |
+|----|------|------|------|------|------|
+| [SeanLee97/angle-llama-13b-nli](https://huggingface.co/SeanLee97/angle-llama-13b-nli) | NousResearch/Llama-2-13b-hf | 4096 | `Prompts.A` | last token | English, Similarity Measurement | 
+| [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-7b-nli-v2) | NousResearch/Llama-2-7b-hf | 4096 | `Prompts.A` | last token | English, Similarity Measurement | 
 
-For example, a sentence semantically similar to "How about ChatGPT?" could be "What is your opinion about ChatGPT?".
 
-To distinguish between these two types of tasks, we use different prompts. 
+## 🚀 Quick Start
 
-For retrieval tasks, we use the prompt "Represent this sentence for searching relevant passages: {text}" (Prompts.C in angle_emb). 
+### ⬇️ Installation
 
-For non-retrieval tasks, we set the prompt to empty, i.e., just input your text without specifying a prompt.
+```bash
+python -m pip install -U angle-emb
+```
 
-So, if your scenario is retrieval-related, it is highly recommended to set the prompt with angle.set_prompt(prompt=Prompts.C). If not, leave the prompt empty or use angle.set_prompt(prompt=None).
-</details>
+### ⌛ Load BERT-based Model
 
-### Angle-LLaMA
+1) **With Prompts**: You can specify a prompt with `prompt=YOUR_PROMPT` in `encode` method. If set a prompt, the inputs should be a list of dict or a single dict with key `text`, where `text` is the placeholder in the prompt for the input text. You can use other placeholder names. We provide a set of predefined prompts in `Prompts` class, you can check them via `Prompts.list_prompts()`.
 
-1) AnglE
 ```python
 from angle_emb import AnglE, Prompts
+from angle_emb.utils import cosine_similarity
 
-angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf', pretrained_lora_path='SeanLee97/angle-llama-7b-nli-v2')
 
-print('All predefined prompts:', Prompts.list_prompts())
-angle.set_prompt(prompt=Prompts.A)
-print('prompt:', angle.prompt)
-vec = angle.encode({'text': 'hello world'}, to_numpy=True)
-print(vec)
-vecs = angle.encode([{'text': 'hello world1'}, {'text': 'hello world2'}], to_numpy=True)
-print(vecs)
+angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1', pooling_strategy='cls').cuda()
+# For retrieval tasks, we use `Prompts.C` as the prompt for the query when using UAE-Large-V1 (no need to specify prompt for documents).
+# When specify prompt, the inputs should be a list of dict with key 'text'
+qv = angle.encode({'text': 'what is the weather?'}, to_numpy=True, prompt=Prompts.C)
+doc_vecs = angle.encode([
+    'The weather is great!',
+    'it is rainy today.',
+    'i am going to bed'
+], to_numpy=True)
+
+for dv in doc_vecs:
+    print(cosine_similarity(qv[0], dv))
 ```
 
-2) transformers
+2) **Without Prompts**: no need to specify a prompt. Just input a list of strings or a single string.
 
 ```python
-from angle_emb import AnglE, Prompts
-from transformers import AutoModelForCausalLM, AutoTokenizer
-from peft import PeftModel, PeftConfig
+from angle_emb import AnglE
+from angle_emb.utils import cosine_similarity
 
-peft_model_id = 'SeanLee97/angle-llama-7b-nli-v2'
-config = PeftConfig.from_pretrained(peft_model_id)
-tokenizer = AutoTokenizer.from_pretrained(config.base_model_name_or_path)
-model = AutoModelForCausalLM.from_pretrained(config.base_model_name_or_path).bfloat16().cuda()
-model = PeftModel.from_pretrained(model, peft_model_id).cuda()
-
-def decorate_text(text: str):
-    return Prompts.A.format(text=text)
-
-inputs = 'hello world!'
-tok = tokenizer([decorate_text(inputs)], return_tensors='pt')
-for k, v in tok.items():
-    tok[k] = v.cuda()
-vec = model(output_hidden_states=True, **tok).hidden_states[-1][:, -1].float().detach().cpu().numpy()
-print(vec)
+
+angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1', pooling_strategy='cls').cuda()
+# for non-retrieval tasks, we don't need to specify prompt when using UAE-Large-V1.
+doc_vecs = angle.encode([
+    'The weather is great!',
+    'The weather is very good!',
+    'i am going to bed'
+])
+
+for i, dv1 in enumerate(doc_vecs):
+    for dv2 in doc_vecs[i+1:]:
+        print(cosine_similarity(dv1, dv2))
 ```
 
-### Angle-BERT
 
-1) AnglE
+### ⌛ Load LLM-based Models
+
+If the pretrained weight is a LoRA-based model, you need to specify the backbone via `model_name_or_path` and specify the LoRA path via the `pretrained_lora_path` in `from_pretrained` method. 
+
 ```python
-from angle_emb import AnglE
+from angle_emb import AnglE, Prompts
 
-angle = AnglE.from_pretrained('SeanLee97/angle-bert-base-uncased-nli-en-v1', pooling_strategy='cls_avg').cuda()
-vec = angle.encode('hello world', to_numpy=True)
+angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
+                              pretrained_lora_path='SeanLee97/angle-llama-7b-nli-v2',
+                              pooling_strategy='last',
+                              is_llm=True,
+                              torch_dtype='float16')
+
+print('All predefined prompts:', Prompts.list_prompts())
+vec = angle.encode({'text': 'hello world'}, to_numpy=True, prompt=Prompts.A)
 print(vec)
-vecs = angle.encode(['hello world1', 'hello world2'], to_numpy=True)
+vecs = angle.encode([{'text': 'hello world1'}, {'text': 'hello world2'}], to_numpy=True, prompt=Prompts.A)
 print(vecs)
 ```
 
-2) transformers
+### ⌛ Load Third-party Models
+
+You can load any transformer-based third-party models such as `mixedbread-ai/mxbai-embed-large-v1`, `sentence-transformers/all-MiniLM-L6-v2`, and `BAAI/bge-large-en-v1.5` using `angle_emb`.
+
+Here is an example:
 
 ```python
-import torch
-from transformers import AutoModel, AutoTokenizer
+from angle_emb import AnglE
 
-model_id = 'SeanLee97/angle-bert-base-uncased-nli-en-v1'
-tokenizer = AutoTokenizer.from_pretrained(model_id)
-model = AutoModel.from_pretrained(model_id).cuda()
-
-inputs = 'hello world!'
-tok = tokenizer([inputs], return_tensors='pt')
-for k, v in tok.items():
-    tok[k] = v.cuda()
-hidden_state = model(**tok).last_hidden_state
-vec = (hidden_state[:, 0] + torch.mean(hidden_state, dim=1)) / 2.0
+model = AnglE.from_pretrained('mixedbread-ai/mxbai-embed-large-v1', pooling_strategy='cls').cuda()
+vec = model.encode('hello world', to_numpy=True)
 print(vec)
 ```
 
-## Custom Train
 
-### 1. Data Prepation
+## 🕸️ Custom Train
+
+### 🗂️ 1. Data Prepation
 
-We support two dataset formats:
+We currently support three dataset formats:
 
 1) `DatasetFormats.A`: it is a pair format with three columns: `text1`, `text2`, and `label` (0/1).
 
 2) `DatasetFormats.B`: it is a triple format with three columns: `text`, `positive`, and `negative`. `positive` and `negative` store the positive and negative samples of `text`.
 
 3) `DatasetFormats.C`: it is a pair format with two columns: `text`, `positive`. `positive` store the positive sample of `text`.
 
 You need to prepare your data into huggingface `datasets.Dataset` in one of the formats in terms of your supervised data.
 
-### 2. Train
+### 🚂 2. Train with CLI
+
+Use `angle-trainer` to train your AnglE model in cli mode. 
+
+1) Single gpu training:
 
-Use `angle-trainer` to train your AnglE model in cli mode. Usage: `CUDA_VISIBLE_DEVICES=0 angle-trainer --help`
+Usage: 
 
+```bash
+CUDA_VISIBLE_DEVICES=0 angle-trainer --help
+```
 
-### 3. Example
+2) Multi-gpu training:
+
+Usage:
+
+```bash
+CUDA_VISIBLE_DEVICES=0,1 torchrun --nproc_per_node=2 --master_port=1234 -m angle_emb.angle_trainer --help
+```
+
+### 🚂 3. Custom Train
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1h28jHvv_x-0fZ0tItIMjf8rJGp3GcO5V?usp=sharing)
 
 
 ```python
 from datasets import load_dataset
 from angle_emb import AnglE, AngleDataTokenizer
@@ -291,45 +259,73 @@
     epochs=5,
     learning_rate=2e-5,
     save_steps=100,
     eval_steps=1000,
     warmup_steps=0,
     gradient_accumulation_steps=1,
     loss_kwargs={
-        'w1': 1.0,
-        'w2': 1.0,
-        'w3': 1.0,
+        'cosine_w': 1.0,
+        'ibn_w': 1.0,
+        'angle_w': 1.0,
         'cosine_tau': 20,
         'ibn_tau': 20,
-        'angle_tau': 1.0
+        'angle_tau': 20
     },
     fp16=True,
     logging_steps=100
 )
 
 # 5. evaluate
 corrcoef, accuracy = angle.evaluate(test_ds, device=angle.device)
 print('corrcoef:', corrcoef)
 ```
 
-# Citation
+### 💡 Others
+
+- To enable `llm` training, please specify `--is_llm 1` and configure appropriate LoRA hyperparameters.
+- To enable `billm` training, please specify `--apply_billm 1` and configure appropriate `billm_model_class` such as `LLamaForCausalLM` (refer to: https://github.com/WhereIsAI/BiLLM?tab=readme-ov-file#usage).
+- To enable espresso sentence embeddings (ESE), please specify `--apply_ese 1` and configure appropriate ESE hyperparameters via `--ese_kl_temperature float` and `--ese_compression_size integer`.
+- To convert the trained AnglE models to `sentence-transformers`, please run `python scripts/convert_to_sentence_transformers.py --help` for more details.
+
+
+## 💡 4. Fine-tuning Tips
+
+1️⃣ If your dataset format is `DatasetFormats.A`, it is recommended to slightly increase the weight for `cosine_w` or slightly decrease the weight for `ibn_w`.
+
+2️⃣ If your dataset format is `DatasetFormats.B`, it is recommended to set `cosine_w` to 0, and increase the weight for `ibn_w` such as 10 and 20. The `angle_tau` is recommended to set to 20.0.
+
+3️⃣ If your dataset format is `DatasetFormats.C`, only `ibn_w` and `ibn_tau` are effective. You don't need to tune other parameters.
+
+4️⃣ To alleviate information forgetting in fine-tuning, it is better to specify the `teacher_name_or_path`. If the `teacher_name_or_path` equals `model_name_or_path`, it will conduct self-distillation. **It is worth to note that** `teacher_name_or_path` has to have the same tokenizer as `model_name_or_path`. Or it will lead to unexpected results.
+
+
+# 🫡 Citation
 
 You are welcome to use our code and pre-trained models. If you use our code and pre-trained models, please support us by citing our work as follows:
 
 ```bibtex
 @article{li2023angle,
   title={AnglE-optimized Text Embeddings},
   author={Li, Xianming and Li, Jing},
   journal={arXiv preprint arXiv:2309.12871},
   year={2023}
 }
 ```
 
-# ChangeLogs
+# 📜 ChangeLogs
 
 | 📅 | Description |
 |----|------|
+| 2024 May 21 |  support Espresso Sentence Embeddings  |
 | 2024 Feb 7 |  support training with only positive pairs (`DatasetFormats.C`)  |
-| 2024 Jan 11 |  refactor to support `angle-trainer` and BeLLM  |
 | 2023 Dec 4 |  Release a universal English sentence embedding model: [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1)  |
 | 2023 Nov 2 |  Release an English pretrained model: `SeanLee97/angle-llama-13b-nli` |
 | 2023 Oct 28 |  Release two chinese pretrained models: `SeanLee97/angle-roberta-wwm-base-zhnli-v1` and `SeanLee97/angle-llama-7b-zhnli-v1`; Add chinese README.md |
+
+# 📧 Contact
+
+If you have any questions or suggestions, please feel free to contact us via email: xmlee97@gmail.com
+
+# © License
+
+This project is licensed under the MIT License.
+For the pretrained models, please refer to the corresponding license of the models.
```

#### html2text {}

```diff
@@ -1,24 +1,20 @@
-Metadata-Version: 2.1 Name: angle_emb Version: 0.3.9 Summary: AnglE-optimize
+Metadata-Version: 2.1 Name: angle-emb Version: 0.4.0 Summary: AnglE-optimize
 Text Embeddings Author: sean lee Author-email: xmlee97@gmail.com Keywords:
 angle_emb Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Description-Content-Type:
 text/markdown License-File: LICENSE EN | [ç®ä½ä¸­æ](README_zh.md) #
-[AnglEð: Angle-optimized Text Embeddings](https://arxiv.org/abs/2309.12871)
-> It is Angle ð, not Angel ð¼. ð¥ **A New SOTA** for Semantic Textual
-Similarity! ð¥ **Our universal sentence embedding [WhereIsAI/UAE-Large-V1]
-(https://huggingface.co/WhereIsAI/UAE-Large-V1) achieves SOTA on the [MTEB
-Leaderboard](https://huggingface.co/spaces/mteb/leaderboard) with an average
-score of 64.64!** _[_h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_3_0_9_._1_2_8_7_1_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I
-_D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_:_/_/_m_a_k_e_a_p_u_l_l_r_e_q_u_e_s_t_._c_o_m_][![PWC](https://img.shields.io/
+AnglEð > It is Angle ð, not Angel ð¼. ð document: https://
+angle.readthedocs.io/en/latest/index.html _[_h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_3_0_9_._1_2_8_7_1_]
+_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _D_o_w_n_l_o_a_d_s_]_[_R_e_a_d_ _t_h_e_ _d_o_c_s_][![PWC](https://img.shields.io/
 endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-
 embeddings/semantic-textual-similarity-on-sick-r-1)](https://
 paperswithcode.com/sota/semantic-textual-similarity-on-sick-r-1?p=angle-
 optimized-text-embeddings) [![PWC](https://img.shields.io/
 endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-
 embeddings/semantic-textual-similarity-on-sts16)](https://paperswithcode.com/
 sota/semantic-textual-similarity-on-sts16?p=angle-optimized-text-embeddings) [!
@@ -35,157 +31,155 @@
 text-embeddings) [![PWC](https://img.shields.io/endpoint.svg?url=https://
 paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-
 similarity-on-sts12)](https://paperswithcode.com/sota/semantic-textual-
 similarity-on-sts12?p=angle-optimized-text-embeddings) [![PWC](https://
 img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-
 optimized-text-embeddings/semantic-textual-similarity-on-sts-benchmark)](https:
 //paperswithcode.com/sota/semantic-textual-similarity-on-sts-benchmark?p=angle-
-optimized-text-embeddings) ð Results on MTEB Leaderboard [click to expand]
-                             [assets/UAE-MTEB.png]
-ð Results on STS benchmark [click to expand]
-                          [assets/angle-results.png]
-## ð¤ Pretrained Models | ð¤ HF | LoRA Weight | Dependent Backbone | LLM |
-Language | Prompt | Pooling Strategy | Examples | |----|------|------|------|--
-----|------|------|------| | [WhereIsAI/UAE-Large-V1](https://huggingface.co/
-WhereIsAI/UAE-Large-V1) | N | N | N | EN | `Prompts.C` for retrieval purposes,
-`None` for others | cls | [![Seach Demo](https://colab.research.google.com/
-assets/colab-badge.svg)](https://colab.research.google.com/drive/
-1WOYD6f8gb_wpkUm_57K8pEDgjlGJd6oB?usp=drive_link) | | [SeanLee97/angle-llama-
-13b-nli](https://huggingface.co/SeanLee97/angle-llama-13b-nli) | Y |
-NousResearch/Llama-2-13b-hf | Y | EN | `Prompts.A` | last token | / | |
+optimized-text-embeddings) ð¢ **Train/Infer Powerful Sentence Embeddings with
+AnglE.** This library is from the paper: [AnglE: Angle-optimized Text
+Embeddings](https://arxiv.org/abs/2309.12871). It allows for training state-of-
+the-art BERT/LLM-based sentence embeddings with just a few lines of code. AnglE
+is also a general sentence embedding inference framework, allowing for infering
+a variety of transformer-based sentence embeddings. ## â¨ Features **Loss**: -
+ð AnglE loss - â Contrastive loss - ð CoSENT loss - âï¸ Espresso
+loss (previously known as 2DMSE, detail: [README_ESE](README_ESE.md))
+**Backbones**: - BERT-based models (BERT, RoBERTa, ELECTRA, ALBERT, etc.) -
+LLM-based models (LLaMA, Mistral, Qwen, etc.) - Bi-directional LLM-based models
+(LLaMA, Mistral, Qwen, OpenELMo, etc.. refer to: https://github.com/WhereIsAI/
+BiLLM) **Training**: - Single-GPU training - Multi-GPU training > _[_h_t_t_p_:_/_/
+_m_a_k_e_a_p_u_l_l_r_e_q_u_e_s_t_._c_o_m_]More features will be added in the future. ## ð
+Achievements ð May 16, 2024 | Paper "[AnglE: Angle-optimized Text
+Embeddings](https://arxiv.org/abs/2309.12871)" is accepted by ACL 2024 Main
+Conference. ð Mar 13, 2024 | Paper "[BeLLM: Backward Dependency Enhanced
+Large Language Model for Sentence Embeddings](https://arxiv.org/abs/
+2311.05296)" is accepted by NAACL 2024 Main Conference. ð Mar 8, 2024 | ð
+[mixedbread's embedding](https://www.mixedbread.ai/blog/mxbai-embed-large-v1) (
+[mixedbread-ai/mxbai-embed-large-v1](https://huggingface.co/mixedbread-ai/
+mxbai-embed-large-v1)) achieves SOTA on the [MTEB Leaderboard](https://
+huggingface.co/spaces/mteb/leaderboard) with an average score of **64.68**! The
+model is trained using AnglE. Congrats mixedbread! ð Dec 4, 2023 | Our
+universal sentence embedding [WhereIsAI/UAE-Large-V1](https://huggingface.co/
+WhereIsAI/UAE-Large-V1) achieves SOTA on the [MTEB Leaderboard](https://
+huggingface.co/spaces/mteb/leaderboard) with an average score of **64.64**! The
+model is trained using AnglE. ð Dec, 2023 | AnglE achieves SOTA performance
+on the STS Bechmark Semantic Textual Similarity! ## ð¤ Official Pretrained
+Models BERT-based models: | ð¤ HF | Max Tokens | Pooling Strategy | Scenario
+| |----|------|------|------| | [WhereIsAI/UAE-Large-V1](https://
+huggingface.co/WhereIsAI/UAE-Large-V1) | 512 | cls | English, General-purpose |
+| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1)
+| 512 | cls | Code Similarity | LLM-based models: | ð¤ HF (lora weight) |
+Backbone | Max Tokens | Prompts | Pooling Strategy | Scenario | |----|------|--
+----|------|------|------| | [SeanLee97/angle-llama-13b-nli](https://
+huggingface.co/SeanLee97/angle-llama-13b-nli) | NousResearch/Llama-2-13b-hf |
+4096 | `Prompts.A` | last token | English, Similarity Measurement | |
 [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-
-7b-nli-v2) | Y | NousResearch/Llama-2-7b-hf | Y | EN | `Prompts.A` | last token
-| / | | [SeanLee97/angle-llama-7b-nli-20231027](https://huggingface.co/
-SeanLee97/angle-llama-7b-nli-20231027) | Y | NousResearch/Llama-2-7b-hf | Y |
-EN | `Prompts.A` | last token | / | | [SeanLee97/angle-bert-base-uncased-nli-
-en-v1](https://huggingface.co/SeanLee97/angle-bert-base-uncased-nli-en-v1) | N
-| N | N | EN | N | `cls_avg` | / | | [SeanLee97/angle-roberta-wwm-base-zhnli-
-v1](https://huggingface.co/SeanLee97/angle-roberta-wwm-base-zhnli-v1) | N | N |
-N | ZH-CN | N | `cls` | / | | [SeanLee97/angle-llama-7b-zhnli-v1](https://
-huggingface.co/SeanLee97/angle-llama-7b-zhnli-v1) | Y | NousResearch/Llama-2-
-7b-hf | Y | ZH-CN | `Prompts.B` | last token | / | ð¡ If the selected model
-is a LoRA weight, it must specify the corresponding dependent backbone. For our
-STS Experiment, please refer to https://github.com/SeanLee97/AnglE/tree/main/
-examples/NLI ## Results ### English STS Results | Model | STS12 | STS13 | STS14
-| STS15 | STS16 | STSBenchmark | SICKRelatedness | Avg. | | ------- |-------|--
------|-------|-------|-------|--------------|-----------------|-------| |
-[SeanLee97/angle-llama-7b-nli-20231027](https://huggingface.co/SeanLee97/angle-
-llama-7b-nli-20231027) | 78.68 | 90.58 | 85.49 | 89.56 | 86.91 | 88.92 | 81.18
-| 85.90 | | [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/
-angle-llama-7b-nli-v2) | 79.00 | 90.56 | 85.79 | 89.43 | 87.00 | 88.97 | 80.94
-| 85.96 | | [SeanLee97/angle-llama-13b-nli](https://huggingface.co/SeanLee97/
-angle-llama-13b-nli) | 79.33 | 90.65 | 86.89 | 90.45 | 87.32 | 89.69 | 81.32 |
-**86.52** | | [SeanLee97/angle-bert-base-uncased-nli-en-v1](https://
-huggingface.co/SeanLee97/angle-bert-base-uncased-nli-en-v1) | 75.09 | 85.56 |
-80.66 | 86.44 | 82.47 | 85.16 | 81.23 | 82.37 | ### Chinese STS Results | Model
-| ATEC | BQ | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc | Avg. | | ------- |---
-----|-------|-------|-------|-------|--------------|-----------------|-------
-| | ^[shibing624/text2vec-bge-large-chinese](https://huggingface.co/shibing624/
-text2vec-bge-large-chinese) | 38.41 | 61.34 | 71.72 | 35.15 | 76.44 | 71.81 |
-63.15 | 59.72 | | ^[shibing624/text2vec-base-chinese-paraphrase](https://
-huggingface.co/shibing624/text2vec-base-chinese-paraphrase) | 44.89 | 63.58 |
-74.24 | 40.90 | 78.93 | 76.70 | 63.30 | 63.08 | | [SeanLee97/angle-roberta-wwm-
-base-zhnli-v1](https://huggingface.co/SeanLee97/angle-roberta-wwm-base-zhnli-
-v1) | 49.49 | 72.47 | 78.33 | 59.13 | 77.14 | 72.36 | 60.53 | **67.06** | |
-[SeanLee97/angle-llama-7b-zhnli-v1](https://huggingface.co/SeanLee97/angle-
-llama-7b-zhnli-v1) | 50.44 | 71.95 | 78.90 | 56.57 | 81.11 | 68.11 | 52.02 |
-65.59 | ^ denotes baselines, their results are retrieved from: https://
-github.com/shibing624/text2vec ## Usage AnglE supports two APIs, one is the
-`transformers` API, the other is the `AnglE` API. If you want to use the
-`AnglE` API, please install AnglE first: ```bash python -m pip install -
-U angle-emb ``` ### UAE 1) For Retrieval Purposes For retrieval purposes,
-please use the prompt `Prompts.C`. ```python from angle_emb import AnglE,
-Prompts angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1',
-pooling_strategy='cls').cuda() angle.set_prompt(prompt=Prompts.C) vec =
-angle.encode({'text': 'hello world'}, to_numpy=True) print(vec) vecs =
-angle.encode([{'text': 'hello world1'}, {'text': 'hello world2'}],
-to_numpy=True) print(vecs) ``` 2) For non-Retrieval Purposes ```python from
-angle_emb import AnglE angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1',
-pooling_strategy='cls').cuda() vec = angle.encode('hello world', to_numpy=True)
-print(vec) vecs = angle.encode(['hello world1', 'hello world2'], to_numpy=True)
-print(vecs) ``` Difference between retrieval and non-retrieval sentence
-embeddings. [click to expand] In UAE, we use different approaches for retrieval
-and non-retrieval tasks, each serving a different purpose. **Retrieval tasks
-aim to find relevant documents, and as a result, the related documents may not
-have strict semantic similarities to each other.** For instance, when querying
-"How about ChatGPT?", the related documents are those that contain information
-related to "ChatGPT," such as "ChatGPT is amazing..." or "ChatGPT is bad....".
-Conversely, **non-retrieval tasks, such as semantic textual similarity, require
-sentences that are semantically similar.** For example, a sentence semantically
-similar to "How about ChatGPT?" could be "What is your opinion about ChatGPT?".
-To distinguish between these two types of tasks, we use different prompts. For
-retrieval tasks, we use the prompt "Represent this sentence for searching
-relevant passages: {text}" (Prompts.C in angle_emb). For non-retrieval tasks,
-we set the prompt to empty, i.e., just input your text without specifying a
-prompt. So, if your scenario is retrieval-related, it is highly recommended to
-set the prompt with angle.set_prompt(prompt=Prompts.C). If not, leave the
-prompt empty or use angle.set_prompt(prompt=None). ### Angle-LLaMA 1) AnglE
-```python from angle_emb import AnglE, Prompts angle = AnglE.from_pretrained
-('NousResearch/Llama-2-7b-hf', pretrained_lora_path='SeanLee97/angle-llama-7b-
-nli-v2') print('All predefined prompts:', Prompts.list_prompts())
-angle.set_prompt(prompt=Prompts.A) print('prompt:', angle.prompt) vec =
-angle.encode({'text': 'hello world'}, to_numpy=True) print(vec) vecs =
-angle.encode([{'text': 'hello world1'}, {'text': 'hello world2'}],
-to_numpy=True) print(vecs) ``` 2) transformers ```python from angle_emb import
-AnglE, Prompts from transformers import AutoModelForCausalLM, AutoTokenizer
-from peft import PeftModel, PeftConfig peft_model_id = 'SeanLee97/angle-llama-
-7b-nli-v2' config = PeftConfig.from_pretrained(peft_model_id) tokenizer =
-AutoTokenizer.from_pretrained(config.base_model_name_or_path) model =
-AutoModelForCausalLM.from_pretrained(config.base_model_name_or_path).bfloat16
-().cuda() model = PeftModel.from_pretrained(model, peft_model_id).cuda() def
-decorate_text(text: str): return Prompts.A.format(text=text) inputs = 'hello
-world!' tok = tokenizer([decorate_text(inputs)], return_tensors='pt') for k, v
-in tok.items(): tok[k] = v.cuda() vec = model(output_hidden_states=True,
-**tok).hidden_states[-1][:, -1].float().detach().cpu().numpy() print(vec) ```
-### Angle-BERT 1) AnglE ```python from angle_emb import AnglE angle =
-AnglE.from_pretrained('SeanLee97/angle-bert-base-uncased-nli-en-v1',
-pooling_strategy='cls_avg').cuda() vec = angle.encode('hello world',
-to_numpy=True) print(vec) vecs = angle.encode(['hello world1', 'hello world2'],
-to_numpy=True) print(vecs) ``` 2) transformers ```python import torch from
-transformers import AutoModel, AutoTokenizer model_id = 'SeanLee97/angle-bert-
-base-uncased-nli-en-v1' tokenizer = AutoTokenizer.from_pretrained(model_id)
-model = AutoModel.from_pretrained(model_id).cuda() inputs = 'hello world!' tok
-= tokenizer([inputs], return_tensors='pt') for k, v in tok.items(): tok[k] =
-v.cuda() hidden_state = model(**tok).last_hidden_state vec = (hidden_state[:,
-0] + torch.mean(hidden_state, dim=1)) / 2.0 print(vec) ``` ## Custom Train ###
-1. Data Prepation We support two dataset formats: 1) `DatasetFormats.A`: it is
-a pair format with three columns: `text1`, `text2`, and `label` (0/1). 2)
+7b-nli-v2) | NousResearch/Llama-2-7b-hf | 4096 | `Prompts.A` | last token |
+English, Similarity Measurement | ## ð Quick Start ### â¬ï¸ Installation
+```bash python -m pip install -U angle-emb ``` ### â Load BERT-based Model 1)
+**With Prompts**: You can specify a prompt with `prompt=YOUR_PROMPT` in
+`encode` method. If set a prompt, the inputs should be a list of dict or a
+single dict with key `text`, where `text` is the placeholder in the prompt for
+the input text. You can use other placeholder names. We provide a set of
+predefined prompts in `Prompts` class, you can check them via
+`Prompts.list_prompts()`. ```python from angle_emb import AnglE, Prompts from
+angle_emb.utils import cosine_similarity angle = AnglE.from_pretrained
+('WhereIsAI/UAE-Large-V1', pooling_strategy='cls').cuda() # For retrieval
+tasks, we use `Prompts.C` as the prompt for the query when using UAE-Large-V1
+(no need to specify prompt for documents). # When specify prompt, the inputs
+should be a list of dict with key 'text' qv = angle.encode({'text': 'what is
+the weather?'}, to_numpy=True, prompt=Prompts.C) doc_vecs = angle.encode([ 'The
+weather is great!', 'it is rainy today.', 'i am going to bed' ], to_numpy=True)
+for dv in doc_vecs: print(cosine_similarity(qv[0], dv)) ``` 2) **Without
+Prompts**: no need to specify a prompt. Just input a list of strings or a
+single string. ```python from angle_emb import AnglE from angle_emb.utils
+import cosine_similarity angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-
+V1', pooling_strategy='cls').cuda() # for non-retrieval tasks, we don't need to
+specify prompt when using UAE-Large-V1. doc_vecs = angle.encode([ 'The weather
+is great!', 'The weather is very good!', 'i am going to bed' ]) for i, dv1 in
+enumerate(doc_vecs): for dv2 in doc_vecs[i+1:]: print(cosine_similarity(dv1,
+dv2)) ``` ### â Load LLM-based Models If the pretrained weight is a LoRA-
+based model, you need to specify the backbone via `model_name_or_path` and
+specify the LoRA path via the `pretrained_lora_path` in `from_pretrained`
+method. ```python from angle_emb import AnglE, Prompts angle =
+AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
+pretrained_lora_path='SeanLee97/angle-llama-7b-nli-v2',
+pooling_strategy='last', is_llm=True, torch_dtype='float16') print('All
+predefined prompts:', Prompts.list_prompts()) vec = angle.encode({'text':
+'hello world'}, to_numpy=True, prompt=Prompts.A) print(vec) vecs = angle.encode
+([{'text': 'hello world1'}, {'text': 'hello world2'}], to_numpy=True,
+prompt=Prompts.A) print(vecs) ``` ### â Load Third-party Models You can load
+any transformer-based third-party models such as `mixedbread-ai/mxbai-embed-
+large-v1`, `sentence-transformers/all-MiniLM-L6-v2`, and `BAAI/bge-large-en-
+v1.5` using `angle_emb`. Here is an example: ```python from angle_emb import
+AnglE model = AnglE.from_pretrained('mixedbread-ai/mxbai-embed-large-v1',
+pooling_strategy='cls').cuda() vec = model.encode('hello world', to_numpy=True)
+print(vec) ``` ## ð¸ï¸ Custom Train ### ðï¸ 1. Data Prepation We
+currently support three dataset formats: 1) `DatasetFormats.A`: it is a pair
+format with three columns: `text1`, `text2`, and `label` (0/1). 2)
 `DatasetFormats.B`: it is a triple format with three columns: `text`,
 `positive`, and `negative`. `positive` and `negative` store the positive and
 negative samples of `text`. 3) `DatasetFormats.C`: it is a pair format with two
 columns: `text`, `positive`. `positive` store the positive sample of `text`.
 You need to prepare your data into huggingface `datasets.Dataset` in one of the
-formats in terms of your supervised data. ### 2. Train Use `angle-trainer` to
-train your AnglE model in cli mode. Usage: `CUDA_VISIBLE_DEVICES=0 angle-
-trainer --help` ### 3. Example [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/1h28jHvv_x-0fZ0tItIMjf8rJGp3GcO5V?usp=sharing)
-```python from datasets import load_dataset from angle_emb import AnglE,
-AngleDataTokenizer # 1. load pretrained model angle = AnglE.from_pretrained
-('SeanLee97/angle-bert-base-uncased-nli-en-v1', max_length=128,
-pooling_strategy='cls').cuda() # 2. load dataset # `text1`, `text2`, and
-`label` are three required columns. ds = load_dataset('mteb/stsbenchmark-sts')
-ds = ds.map(lambda obj: {"text1": str(obj["sentence1"]), "text2": str(obj
-['sentence2']), "label": obj['score']}) ds = ds.select_columns(["text1",
-"text2", "label"]) # 3. transform data train_ds = ds['train'].shuffle().map
-(AngleDataTokenizer(angle.tokenizer, angle.max_length), num_proc=8) valid_ds =
-ds['validation'].map(AngleDataTokenizer(angle.tokenizer, angle.max_length),
-num_proc=8) test_ds = ds['test'].map(AngleDataTokenizer(angle.tokenizer,
-angle.max_length), num_proc=8) # 4. fit angle.fit( train_ds=train_ds,
-valid_ds=valid_ds, output_dir='ckpts/sts-b', batch_size=32, epochs=5,
-learning_rate=2e-5, save_steps=100, eval_steps=1000, warmup_steps=0,
-gradient_accumulation_steps=1, loss_kwargs={ 'w1': 1.0, 'w2': 1.0, 'w3': 1.0,
-'cosine_tau': 20, 'ibn_tau': 20, 'angle_tau': 1.0 }, fp16=True,
-logging_steps=100 ) # 5. evaluate corrcoef, accuracy = angle.evaluate(test_ds,
-device=angle.device) print('corrcoef:', corrcoef) ``` # Citation You are
-welcome to use our code and pre-trained models. If you use our code and pre-
-trained models, please support us by citing our work as follows: ```bibtex
-@article{li2023angle, title={AnglE-optimized Text Embeddings}, author={Li,
-Xianming and Li, Jing}, journal={arXiv preprint arXiv:2309.12871}, year={2023}
-} ``` # ChangeLogs | ð | Description | |----|------| | 2024 Feb 7 | support
-training with only positive pairs (`DatasetFormats.C`) | | 2024 Jan 11 |
-refactor to support `angle-trainer` and BeLLM | | 2023 Dec 4 | Release a
-universal English sentence embedding model: [WhereIsAI/UAE-Large-V1](https://
-huggingface.co/WhereIsAI/UAE-Large-V1) | | 2023 Nov 2 | Release an English
-pretrained model: `SeanLee97/angle-llama-13b-nli` | | 2023 Oct 28 | Release two
-chinese pretrained models: `SeanLee97/angle-roberta-wwm-base-zhnli-v1` and
-`SeanLee97/angle-llama-7b-zhnli-v1`; Add chinese README.md |
+formats in terms of your supervised data. ### ð 2. Train with CLI Use
+`angle-trainer` to train your AnglE model in cli mode. 1) Single gpu training:
+Usage: ```bash CUDA_VISIBLE_DEVICES=0 angle-trainer --help ``` 2) Multi-gpu
+training: Usage: ```bash CUDA_VISIBLE_DEVICES=0,1 torchrun --nproc_per_node=2 -
+-master_port=1234 -m angle_emb.angle_trainer --help ``` ### ð 3. Custom
+Train [![Open In Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/drive/1h28jHvv_x-
+0fZ0tItIMjf8rJGp3GcO5V?usp=sharing) ```python from datasets import load_dataset
+from angle_emb import AnglE, AngleDataTokenizer # 1. load pretrained model
+angle = AnglE.from_pretrained('SeanLee97/angle-bert-base-uncased-nli-en-v1',
+max_length=128, pooling_strategy='cls').cuda() # 2. load dataset # `text1`,
+`text2`, and `label` are three required columns. ds = load_dataset('mteb/
+stsbenchmark-sts') ds = ds.map(lambda obj: {"text1": str(obj["sentence1"]),
+"text2": str(obj['sentence2']), "label": obj['score']}) ds = ds.select_columns(
+["text1", "text2", "label"]) # 3. transform data train_ds = ds['train'].shuffle
+().map(AngleDataTokenizer(angle.tokenizer, angle.max_length), num_proc=8)
+valid_ds = ds['validation'].map(AngleDataTokenizer(angle.tokenizer,
+angle.max_length), num_proc=8) test_ds = ds['test'].map(AngleDataTokenizer
+(angle.tokenizer, angle.max_length), num_proc=8) # 4. fit angle.fit
+( train_ds=train_ds, valid_ds=valid_ds, output_dir='ckpts/sts-b',
+batch_size=32, epochs=5, learning_rate=2e-5, save_steps=100, eval_steps=1000,
+warmup_steps=0, gradient_accumulation_steps=1, loss_kwargs={ 'cosine_w': 1.0,
+'ibn_w': 1.0, 'angle_w': 1.0, 'cosine_tau': 20, 'ibn_tau': 20, 'angle_tau': 20
+}, fp16=True, logging_steps=100 ) # 5. evaluate corrcoef, accuracy =
+angle.evaluate(test_ds, device=angle.device) print('corrcoef:', corrcoef) ```
+### ð¡ Others - To enable `llm` training, please specify `--is_llm 1` and
+configure appropriate LoRA hyperparameters. - To enable `billm` training,
+please specify `--apply_billm 1` and configure appropriate `billm_model_class`
+such as `LLamaForCausalLM` (refer to: https://github.com/WhereIsAI/
+BiLLM?tab=readme-ov-file#usage). - To enable espresso sentence embeddings
+(ESE), please specify `--apply_ese 1` and configure appropriate ESE
+hyperparameters via `--ese_kl_temperature float` and `--ese_compression_size
+integer`. - To convert the trained AnglE models to `sentence-transformers`,
+please run `python scripts/convert_to_sentence_transformers.py --help` for more
+details. ## ð¡ 4. Fine-tuning Tips 1ï¸â£ If your dataset format is
+`DatasetFormats.A`, it is recommended to slightly increase the weight for
+`cosine_w` or slightly decrease the weight for `ibn_w`. 2ï¸â£ If your dataset
+format is `DatasetFormats.B`, it is recommended to set `cosine_w` to 0, and
+increase the weight for `ibn_w` such as 10 and 20. The `angle_tau` is
+recommended to set to 20.0. 3ï¸â£ If your dataset format is
+`DatasetFormats.C`, only `ibn_w` and `ibn_tau` are effective. You don't need to
+tune other parameters. 4ï¸â£ To alleviate information forgetting in fine-
+tuning, it is better to specify the `teacher_name_or_path`. If the
+`teacher_name_or_path` equals `model_name_or_path`, it will conduct self-
+distillation. **It is worth to note that** `teacher_name_or_path` has to have
+the same tokenizer as `model_name_or_path`. Or it will lead to unexpected
+results. # ð«¡ Citation You are welcome to use our code and pre-trained
+models. If you use our code and pre-trained models, please support us by citing
+our work as follows: ```bibtex @article{li2023angle, title={AnglE-optimized
+Text Embeddings}, author={Li, Xianming and Li, Jing}, journal={arXiv preprint
+arXiv:2309.12871}, year={2023} } ``` # ð ChangeLogs | ð | Description |
+|----|------| | 2024 May 21 | support Espresso Sentence Embeddings | | 2024 Feb
+7 | support training with only positive pairs (`DatasetFormats.C`) | | 2023 Dec
+4 | Release a universal English sentence embedding model: [WhereIsAI/UAE-Large-
+V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) | | 2023 Nov 2 | Release an
+English pretrained model: `SeanLee97/angle-llama-13b-nli` | | 2023 Oct 28 |
+Release two chinese pretrained models: `SeanLee97/angle-roberta-wwm-base-zhnli-
+v1` and `SeanLee97/angle-llama-7b-zhnli-v1`; Add chinese README.md | # ð§
+Contact If you have any questions or suggestions, please feel free to contact
+us via email: xmlee97@gmail.com # Â© License This project is licensed under the
+MIT License. For the pretrained models, please refer to the corresponding
+license of the models.
```

### Comparing `angle_emb-0.3.9/README.md` & `angle_emb-0.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,248 +1,216 @@
 <small>EN | [简体中文](README_zh.md) </small>
 
-# [AnglE📐: Angle-optimized Text Embeddings](https://arxiv.org/abs/2309.12871)
+# AnglE📐
 
 > It is Angle 📐, not Angel 👼.
 
-🔥 **A New SOTA** for Semantic Textual Similarity! 
-
-
-🔥 **Our universal sentence embedding [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) achieves SOTA on the [MTEB Leaderboard](https://huggingface.co/spaces/mteb/leaderboard) with an average score of 64.64!**
-
+📘 document: https://angle.readthedocs.io/en/latest/index.html
 
 <a href="https://arxiv.org/abs/2309.12871">
-    <img src="https://img.shields.io/badge/Arxiv-2306.06843-yellow.svg?style=flat-square" alt="https://arxiv.org/abs/2309.12871" />
+    <img src="https://img.shields.io/badge/Arxiv-2309.12871-yellow.svg?style=flat-square" alt="https://arxiv.org/abs/2309.12871" />
 </a>
 <a href="https://pypi.org/project/angle_emb/">
     <img src="https://img.shields.io/pypi/v/angle_emb?style=flat-square" alt="PyPI version" />
 </a>
 <a href="https://pypi.org/project/angle_emb/">
     <img src="https://img.shields.io/pypi/dm/angle_emb?style=flat-square" alt="PyPI Downloads" />
 </a>
-<a href="http://makeapullrequest.com">
-    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="http://makeapullrequest.com" />
+<a href="https://angle.readthedocs.io/en/latest/index.html">
+    <img src="https://readthedocs.org/projects/angle/badge/?version=latest&style=flat-square" alt="Read the docs" />
 </a>
 
+
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sick-r-1)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sick-r-1?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts16)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts16?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts15)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts15?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts14)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts14?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts13)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts13?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts12)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts12?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts-benchmark)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts-benchmark?p=angle-optimized-text-embeddings)
 
+📢 **Train/Infer Powerful Sentence Embeddings with AnglE.**
+This library is from the paper: [AnglE: Angle-optimized Text Embeddings](https://arxiv.org/abs/2309.12871). It allows for training state-of-the-art BERT/LLM-based sentence embeddings with just a few lines of code. AnglE is also a general sentence embedding inference framework, allowing for infering a variety of transformer-based sentence embeddings.
 
-<details>
-<summary>📊 Results on MTEB Leaderboard [click to expand]</summary>
-<p align='center'>
-<img src='assets/UAE-MTEB.png'>
-</p>
-</details>
-
-<details>
-<summary>📊 Results on STS benchmark [click to expand]</summary>
-<p align='center'>
-<img src='assets/angle-results.png'>
-</p>
-</details>
-
-## 🤗 Pretrained Models
-| 🤗 HF | LoRA Weight | Dependent Backbone | LLM | Language | Prompt | Pooling Strategy | Examples |
-|----|------|------|------|------|------|------|------|
-| [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) |  N | N | N | EN | `Prompts.C` for retrieval purposes, `None` for others | cls | [![Seach Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WOYD6f8gb_wpkUm_57K8pEDgjlGJd6oB?usp=drive_link) |
-| [SeanLee97/angle-llama-13b-nli](https://huggingface.co/SeanLee97/angle-llama-13b-nli) | Y |  NousResearch/Llama-2-13b-hf | Y | EN | `Prompts.A` | last token | / | 
-| [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-7b-nli-v2) | Y |  NousResearch/Llama-2-7b-hf | Y | EN | `Prompts.A` | last token | / |
-| [SeanLee97/angle-llama-7b-nli-20231027](https://huggingface.co/SeanLee97/angle-llama-7b-nli-20231027) | Y |  NousResearch/Llama-2-7b-hf | Y | EN | `Prompts.A` | last token | / |
-| [SeanLee97/angle-bert-base-uncased-nli-en-v1](https://huggingface.co/SeanLee97/angle-bert-base-uncased-nli-en-v1) | N |  N | N | EN | N | `cls_avg` | / |
-| [SeanLee97/angle-roberta-wwm-base-zhnli-v1](https://huggingface.co/SeanLee97/angle-roberta-wwm-base-zhnli-v1) | N |  N | N | ZH-CN | N | `cls` | / |
-| [SeanLee97/angle-llama-7b-zhnli-v1](https://huggingface.co/SeanLee97/angle-llama-7b-zhnli-v1) | Y |  NousResearch/Llama-2-7b-hf | Y | ZH-CN | `Prompts.B` | last token | / |
- 
-💡 If the selected model is a LoRA weight, it must specify the corresponding dependent backbone.
-
-For our STS Experiment, please refer to https://github.com/SeanLee97/AnglE/tree/main/examples/NLI
-
-</details>
-
-## Results
-
-### English STS Results
-
-| Model | STS12 | STS13 | STS14 | STS15 | STS16 | STSBenchmark | SICKRelatedness |  Avg. |
-| ------- |-------|-------|-------|-------|-------|--------------|-----------------|-------|
-| [SeanLee97/angle-llama-7b-nli-20231027](https://huggingface.co/SeanLee97/angle-llama-7b-nli-20231027) | 78.68 | 90.58 | 85.49 | 89.56 | 86.91 |    88.92     |      81.18      | 85.90 |
-| [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-7b-nli-v2) | 79.00 | 90.56 | 85.79 | 89.43 | 87.00 |    88.97     |      80.94      | 85.96 |
-| [SeanLee97/angle-llama-13b-nli](https://huggingface.co/SeanLee97/angle-llama-13b-nli)  | 79.33 | 90.65 | 86.89 | 90.45 | 87.32 |    89.69     |      81.32       | **86.52** |
-| [SeanLee97/angle-bert-base-uncased-nli-en-v1](https://huggingface.co/SeanLee97/angle-bert-base-uncased-nli-en-v1) | 75.09 | 85.56 | 80.66 | 86.44 | 82.47 | 85.16 | 81.23 | 82.37 |
-
-
-### Chinese STS Results
-
-| Model | ATEC | BQ	| LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc | Avg. |
-| ------- |-------|-------|-------|-------|-------|--------------|-----------------|-------|
-| ^[shibing624/text2vec-bge-large-chinese](https://huggingface.co/shibing624/text2vec-bge-large-chinese) | 38.41 | 61.34 | 71.72 | 35.15 | 76.44 | 71.81 | 63.15 | 59.72 |
-| ^[shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase) |	44.89 | 63.58 | 74.24 | 40.90 | 78.93 | 76.70 | 63.30 | 63.08 |
-| [SeanLee97/angle-roberta-wwm-base-zhnli-v1](https://huggingface.co/SeanLee97/angle-roberta-wwm-base-zhnli-v1) | 49.49 | 72.47 | 78.33 | 59.13 | 77.14 |    72.36     |      60.53      | **67.06** |
-| [SeanLee97/angle-llama-7b-zhnli-v1](https://huggingface.co/SeanLee97/angle-llama-7b-zhnli-v1) | 50.44 | 71.95 | 78.90 | 56.57 | 81.11 | 68.11 | 52.02 | 65.59 |
+## ✨ Features
 
-^ denotes baselines, their results are retrieved from: https://github.com/shibing624/text2vec
+**Loss**:
+- 📐 AnglE loss
+- ⚖ Contrastive loss
+- 📏 CoSENT loss
+- ☕️ Espresso loss (previously known as 2DMSE, detail: [README_ESE](README_ESE.md))
 
+**Backbones**:
+- BERT-based models (BERT, RoBERTa, ELECTRA, ALBERT, etc.)
+- LLM-based models (LLaMA, Mistral, Qwen, etc.)
+- Bi-directional LLM-based models (LLaMA, Mistral, Qwen, OpenELMo, etc.. refer to: https://github.com/WhereIsAI/BiLLM)
 
-## Usage
+**Training**:
+- Single-GPU training
+- Multi-GPU training
 
-AnglE supports two APIs, one is the `transformers` API, the other is the `AnglE` API. If you want to use the `AnglE` API, please install AnglE first:
 
-```bash
-python -m pip install -U angle-emb
-```
+> <a href="http://makeapullrequest.com"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="http://makeapullrequest.com" /></a> 
+    More features will be added in the future. 
 
-### UAE
+## 🏆 Achievements
 
-1) For Retrieval Purposes
+📅  May 16, 2024 | Paper "[AnglE: Angle-optimized Text Embeddings](https://arxiv.org/abs/2309.12871)" is accepted by ACL 2024 Main Conference.
 
-For retrieval purposes, please use the prompt `Prompts.C`.
+📅  Mar 13, 2024 | Paper "[BeLLM: Backward Dependency Enhanced Large Language Model for Sentence Embeddings](https://arxiv.org/abs/2311.05296)" is accepted by NAACL 2024 Main Conference.
 
-```python
-from angle_emb import AnglE, Prompts
 
-angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1', pooling_strategy='cls').cuda()
-angle.set_prompt(prompt=Prompts.C)
-vec = angle.encode({'text': 'hello world'}, to_numpy=True)
-print(vec)
-vecs = angle.encode([{'text': 'hello world1'}, {'text': 'hello world2'}], to_numpy=True)
-print(vecs)
-```
+📅  Mar 8, 2024 | 🍞 [mixedbread's embedding](https://www.mixedbread.ai/blog/mxbai-embed-large-v1) ([mixedbread-ai/mxbai-embed-large-v1](https://huggingface.co/mixedbread-ai/mxbai-embed-large-v1)) achieves SOTA on the [MTEB Leaderboard](https://huggingface.co/spaces/mteb/leaderboard) with an average score of **64.68**! The model is trained using AnglE. Congrats mixedbread!
 
-2) For non-Retrieval Purposes
 
-```python
-from angle_emb import AnglE
+📅  Dec 4, 2023 | Our universal sentence embedding [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) achieves SOTA on the [MTEB Leaderboard](https://huggingface.co/spaces/mteb/leaderboard) with an average score of **64.64**! The model is trained using AnglE.
+
+
+📅 Dec, 2023 | AnglE achieves SOTA performance on the STS Bechmark Semantic Textual Similarity! 
 
-angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1', pooling_strategy='cls').cuda()
-vec = angle.encode('hello world', to_numpy=True)
-print(vec)
-vecs = angle.encode(['hello world1', 'hello world2'], to_numpy=True)
-print(vecs)
-```
 
-<details>
-<summary>Difference between retrieval and non-retrieval sentence embeddings. [click to expand]</summary>
+## 🤗 Official Pretrained Models
 
-In UAE, we use different approaches for retrieval and non-retrieval tasks, each serving a different purpose. 
+BERT-based models:
 
-**Retrieval tasks aim to find relevant documents, and as a result, the related documents may not have strict semantic similarities to each other.**
+|  🤗 HF | Max Tokens | Pooling Strategy | Scenario |
+|----|------|------|------|
+| [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) | 512 | cls | English, General-purpose |
+| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) |  512 | cls | Code Similarity |
 
-For instance, when querying "How about ChatGPT?", the related documents are those that contain information related to "ChatGPT," such as "ChatGPT is amazing..." or "ChatGPT is bad....".
+LLM-based models:
 
-Conversely, **non-retrieval tasks, such as semantic textual similarity, require sentences that are semantically similar.**
+| 🤗 HF (lora weight) | Backbone | Max Tokens | Prompts |  Pooling Strategy | Scenario  |
+|----|------|------|------|------|------|
+| [SeanLee97/angle-llama-13b-nli](https://huggingface.co/SeanLee97/angle-llama-13b-nli) | NousResearch/Llama-2-13b-hf | 4096 | `Prompts.A` | last token | English, Similarity Measurement | 
+| [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-7b-nli-v2) | NousResearch/Llama-2-7b-hf | 4096 | `Prompts.A` | last token | English, Similarity Measurement | 
 
-For example, a sentence semantically similar to "How about ChatGPT?" could be "What is your opinion about ChatGPT?".
 
-To distinguish between these two types of tasks, we use different prompts. 
+## 🚀 Quick Start
 
-For retrieval tasks, we use the prompt "Represent this sentence for searching relevant passages: {text}" (Prompts.C in angle_emb). 
+### ⬇️ Installation
 
-For non-retrieval tasks, we set the prompt to empty, i.e., just input your text without specifying a prompt.
+```bash
+python -m pip install -U angle-emb
+```
 
-So, if your scenario is retrieval-related, it is highly recommended to set the prompt with angle.set_prompt(prompt=Prompts.C). If not, leave the prompt empty or use angle.set_prompt(prompt=None).
-</details>
+### ⌛ Load BERT-based Model
 
-### Angle-LLaMA
+1) **With Prompts**: You can specify a prompt with `prompt=YOUR_PROMPT` in `encode` method. If set a prompt, the inputs should be a list of dict or a single dict with key `text`, where `text` is the placeholder in the prompt for the input text. You can use other placeholder names. We provide a set of predefined prompts in `Prompts` class, you can check them via `Prompts.list_prompts()`.
 
-1) AnglE
 ```python
 from angle_emb import AnglE, Prompts
+from angle_emb.utils import cosine_similarity
 
-angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf', pretrained_lora_path='SeanLee97/angle-llama-7b-nli-v2')
 
-print('All predefined prompts:', Prompts.list_prompts())
-angle.set_prompt(prompt=Prompts.A)
-print('prompt:', angle.prompt)
-vec = angle.encode({'text': 'hello world'}, to_numpy=True)
-print(vec)
-vecs = angle.encode([{'text': 'hello world1'}, {'text': 'hello world2'}], to_numpy=True)
-print(vecs)
+angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1', pooling_strategy='cls').cuda()
+# For retrieval tasks, we use `Prompts.C` as the prompt for the query when using UAE-Large-V1 (no need to specify prompt for documents).
+# When specify prompt, the inputs should be a list of dict with key 'text'
+qv = angle.encode({'text': 'what is the weather?'}, to_numpy=True, prompt=Prompts.C)
+doc_vecs = angle.encode([
+    'The weather is great!',
+    'it is rainy today.',
+    'i am going to bed'
+], to_numpy=True)
+
+for dv in doc_vecs:
+    print(cosine_similarity(qv[0], dv))
 ```
 
-2) transformers
+2) **Without Prompts**: no need to specify a prompt. Just input a list of strings or a single string.
 
 ```python
-from angle_emb import AnglE, Prompts
-from transformers import AutoModelForCausalLM, AutoTokenizer
-from peft import PeftModel, PeftConfig
+from angle_emb import AnglE
+from angle_emb.utils import cosine_similarity
 
-peft_model_id = 'SeanLee97/angle-llama-7b-nli-v2'
-config = PeftConfig.from_pretrained(peft_model_id)
-tokenizer = AutoTokenizer.from_pretrained(config.base_model_name_or_path)
-model = AutoModelForCausalLM.from_pretrained(config.base_model_name_or_path).bfloat16().cuda()
-model = PeftModel.from_pretrained(model, peft_model_id).cuda()
-
-def decorate_text(text: str):
-    return Prompts.A.format(text=text)
-
-inputs = 'hello world!'
-tok = tokenizer([decorate_text(inputs)], return_tensors='pt')
-for k, v in tok.items():
-    tok[k] = v.cuda()
-vec = model(output_hidden_states=True, **tok).hidden_states[-1][:, -1].float().detach().cpu().numpy()
-print(vec)
+
+angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1', pooling_strategy='cls').cuda()
+# for non-retrieval tasks, we don't need to specify prompt when using UAE-Large-V1.
+doc_vecs = angle.encode([
+    'The weather is great!',
+    'The weather is very good!',
+    'i am going to bed'
+])
+
+for i, dv1 in enumerate(doc_vecs):
+    for dv2 in doc_vecs[i+1:]:
+        print(cosine_similarity(dv1, dv2))
 ```
 
-### Angle-BERT
 
-1) AnglE
+### ⌛ Load LLM-based Models
+
+If the pretrained weight is a LoRA-based model, you need to specify the backbone via `model_name_or_path` and specify the LoRA path via the `pretrained_lora_path` in `from_pretrained` method. 
+
 ```python
-from angle_emb import AnglE
+from angle_emb import AnglE, Prompts
 
-angle = AnglE.from_pretrained('SeanLee97/angle-bert-base-uncased-nli-en-v1', pooling_strategy='cls_avg').cuda()
-vec = angle.encode('hello world', to_numpy=True)
+angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
+                              pretrained_lora_path='SeanLee97/angle-llama-7b-nli-v2',
+                              pooling_strategy='last',
+                              is_llm=True,
+                              torch_dtype='float16')
+
+print('All predefined prompts:', Prompts.list_prompts())
+vec = angle.encode({'text': 'hello world'}, to_numpy=True, prompt=Prompts.A)
 print(vec)
-vecs = angle.encode(['hello world1', 'hello world2'], to_numpy=True)
+vecs = angle.encode([{'text': 'hello world1'}, {'text': 'hello world2'}], to_numpy=True, prompt=Prompts.A)
 print(vecs)
 ```
 
-2) transformers
+### ⌛ Load Third-party Models
+
+You can load any transformer-based third-party models such as `mixedbread-ai/mxbai-embed-large-v1`, `sentence-transformers/all-MiniLM-L6-v2`, and `BAAI/bge-large-en-v1.5` using `angle_emb`.
+
+Here is an example:
 
 ```python
-import torch
-from transformers import AutoModel, AutoTokenizer
+from angle_emb import AnglE
 
-model_id = 'SeanLee97/angle-bert-base-uncased-nli-en-v1'
-tokenizer = AutoTokenizer.from_pretrained(model_id)
-model = AutoModel.from_pretrained(model_id).cuda()
-
-inputs = 'hello world!'
-tok = tokenizer([inputs], return_tensors='pt')
-for k, v in tok.items():
-    tok[k] = v.cuda()
-hidden_state = model(**tok).last_hidden_state
-vec = (hidden_state[:, 0] + torch.mean(hidden_state, dim=1)) / 2.0
+model = AnglE.from_pretrained('mixedbread-ai/mxbai-embed-large-v1', pooling_strategy='cls').cuda()
+vec = model.encode('hello world', to_numpy=True)
 print(vec)
 ```
 
-## Custom Train
 
-### 1. Data Prepation
+## 🕸️ Custom Train
+
+### 🗂️ 1. Data Prepation
 
-We support two dataset formats:
+We currently support three dataset formats:
 
 1) `DatasetFormats.A`: it is a pair format with three columns: `text1`, `text2`, and `label` (0/1).
 
 2) `DatasetFormats.B`: it is a triple format with three columns: `text`, `positive`, and `negative`. `positive` and `negative` store the positive and negative samples of `text`.
 
 3) `DatasetFormats.C`: it is a pair format with two columns: `text`, `positive`. `positive` store the positive sample of `text`.
 
 You need to prepare your data into huggingface `datasets.Dataset` in one of the formats in terms of your supervised data.
 
-### 2. Train
+### 🚂 2. Train with CLI
+
+Use `angle-trainer` to train your AnglE model in cli mode. 
+
+1) Single gpu training:
 
-Use `angle-trainer` to train your AnglE model in cli mode. Usage: `CUDA_VISIBLE_DEVICES=0 angle-trainer --help`
+Usage: 
 
+```bash
+CUDA_VISIBLE_DEVICES=0 angle-trainer --help
+```
 
-### 3. Example
+2) Multi-gpu training:
+
+Usage:
+
+```bash
+CUDA_VISIBLE_DEVICES=0,1 torchrun --nproc_per_node=2 --master_port=1234 -m angle_emb.angle_trainer --help
+```
+
+### 🚂 3. Custom Train
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1h28jHvv_x-0fZ0tItIMjf8rJGp3GcO5V?usp=sharing)
 
 
 ```python
 from datasets import load_dataset
 from angle_emb import AnglE, AngleDataTokenizer
@@ -271,45 +239,73 @@
     epochs=5,
     learning_rate=2e-5,
     save_steps=100,
     eval_steps=1000,
     warmup_steps=0,
     gradient_accumulation_steps=1,
     loss_kwargs={
-        'w1': 1.0,
-        'w2': 1.0,
-        'w3': 1.0,
+        'cosine_w': 1.0,
+        'ibn_w': 1.0,
+        'angle_w': 1.0,
         'cosine_tau': 20,
         'ibn_tau': 20,
-        'angle_tau': 1.0
+        'angle_tau': 20
     },
     fp16=True,
     logging_steps=100
 )
 
 # 5. evaluate
 corrcoef, accuracy = angle.evaluate(test_ds, device=angle.device)
 print('corrcoef:', corrcoef)
 ```
 
-# Citation
+### 💡 Others
+
+- To enable `llm` training, please specify `--is_llm 1` and configure appropriate LoRA hyperparameters.
+- To enable `billm` training, please specify `--apply_billm 1` and configure appropriate `billm_model_class` such as `LLamaForCausalLM` (refer to: https://github.com/WhereIsAI/BiLLM?tab=readme-ov-file#usage).
+- To enable espresso sentence embeddings (ESE), please specify `--apply_ese 1` and configure appropriate ESE hyperparameters via `--ese_kl_temperature float` and `--ese_compression_size integer`.
+- To convert the trained AnglE models to `sentence-transformers`, please run `python scripts/convert_to_sentence_transformers.py --help` for more details.
+
+
+## 💡 4. Fine-tuning Tips
+
+1️⃣ If your dataset format is `DatasetFormats.A`, it is recommended to slightly increase the weight for `cosine_w` or slightly decrease the weight for `ibn_w`.
+
+2️⃣ If your dataset format is `DatasetFormats.B`, it is recommended to set `cosine_w` to 0, and increase the weight for `ibn_w` such as 10 and 20. The `angle_tau` is recommended to set to 20.0.
+
+3️⃣ If your dataset format is `DatasetFormats.C`, only `ibn_w` and `ibn_tau` are effective. You don't need to tune other parameters.
+
+4️⃣ To alleviate information forgetting in fine-tuning, it is better to specify the `teacher_name_or_path`. If the `teacher_name_or_path` equals `model_name_or_path`, it will conduct self-distillation. **It is worth to note that** `teacher_name_or_path` has to have the same tokenizer as `model_name_or_path`. Or it will lead to unexpected results.
+
+
+# 🫡 Citation
 
 You are welcome to use our code and pre-trained models. If you use our code and pre-trained models, please support us by citing our work as follows:
 
 ```bibtex
 @article{li2023angle,
   title={AnglE-optimized Text Embeddings},
   author={Li, Xianming and Li, Jing},
   journal={arXiv preprint arXiv:2309.12871},
   year={2023}
 }
 ```
 
-# ChangeLogs
+# 📜 ChangeLogs
 
 | 📅 | Description |
 |----|------|
+| 2024 May 21 |  support Espresso Sentence Embeddings  |
 | 2024 Feb 7 |  support training with only positive pairs (`DatasetFormats.C`)  |
-| 2024 Jan 11 |  refactor to support `angle-trainer` and BeLLM  |
 | 2023 Dec 4 |  Release a universal English sentence embedding model: [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1)  |
 | 2023 Nov 2 |  Release an English pretrained model: `SeanLee97/angle-llama-13b-nli` |
 | 2023 Oct 28 |  Release two chinese pretrained models: `SeanLee97/angle-roberta-wwm-base-zhnli-v1` and `SeanLee97/angle-llama-7b-zhnli-v1`; Add chinese README.md |
+
+# 📧 Contact
+
+If you have any questions or suggestions, please feel free to contact us via email: xmlee97@gmail.com
+
+# © License
+
+This project is licensed under the MIT License.
+For the pretrained models, please refer to the corresponding license of the models.
```

#### html2text {}

```diff
@@ -1,15 +1,11 @@
-EN | [ç®ä½ä¸­æ](README_zh.md) # [AnglEð: Angle-optimized Text
-Embeddings](https://arxiv.org/abs/2309.12871) > It is Angle ð, not Angel
-ð¼. ð¥ **A New SOTA** for Semantic Textual Similarity! ð¥ **Our universal
-sentence embedding [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/
-UAE-Large-V1) achieves SOTA on the [MTEB Leaderboard](https://huggingface.co/
-spaces/mteb/leaderboard) with an average score of 64.64!** _[_h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/
-_a_b_s_/_2_3_0_9_._1_2_8_7_1_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_:_/_/_m_a_k_e_a_p_u_l_l_r_e_q_u_e_s_t_._c_o_m_][!
-[PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/
+EN | [ç®ä½ä¸­æ](README_zh.md) # AnglEð > It is Angle ð, not Angel
+ð¼. ð document: https://angle.readthedocs.io/en/latest/index.html _[_h_t_t_p_s_:_/
+_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_3_0_9_._1_2_8_7_1_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _D_o_w_n_l_o_a_d_s_]_[_R_e_a_d_ _t_h_e_ _d_o_c_s_][![PWC]
+(https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/
 angle-optimized-text-embeddings/semantic-textual-similarity-on-sick-r-1)]
 (https://paperswithcode.com/sota/semantic-textual-similarity-on-sick-r-
 1?p=angle-optimized-text-embeddings) [![PWC](https://img.shields.io/
 endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-
 embeddings/semantic-textual-similarity-on-sts16)](https://paperswithcode.com/
 sota/semantic-textual-similarity-on-sts16?p=angle-optimized-text-embeddings) [!
 [PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/
@@ -25,157 +21,155 @@
 text-embeddings) [![PWC](https://img.shields.io/endpoint.svg?url=https://
 paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-
 similarity-on-sts12)](https://paperswithcode.com/sota/semantic-textual-
 similarity-on-sts12?p=angle-optimized-text-embeddings) [![PWC](https://
 img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-
 optimized-text-embeddings/semantic-textual-similarity-on-sts-benchmark)](https:
 //paperswithcode.com/sota/semantic-textual-similarity-on-sts-benchmark?p=angle-
-optimized-text-embeddings) ð Results on MTEB Leaderboard [click to expand]
-                             [assets/UAE-MTEB.png]
-ð Results on STS benchmark [click to expand]
-                          [assets/angle-results.png]
-## ð¤ Pretrained Models | ð¤ HF | LoRA Weight | Dependent Backbone | LLM |
-Language | Prompt | Pooling Strategy | Examples | |----|------|------|------|--
-----|------|------|------| | [WhereIsAI/UAE-Large-V1](https://huggingface.co/
-WhereIsAI/UAE-Large-V1) | N | N | N | EN | `Prompts.C` for retrieval purposes,
-`None` for others | cls | [![Seach Demo](https://colab.research.google.com/
-assets/colab-badge.svg)](https://colab.research.google.com/drive/
-1WOYD6f8gb_wpkUm_57K8pEDgjlGJd6oB?usp=drive_link) | | [SeanLee97/angle-llama-
-13b-nli](https://huggingface.co/SeanLee97/angle-llama-13b-nli) | Y |
-NousResearch/Llama-2-13b-hf | Y | EN | `Prompts.A` | last token | / | |
+optimized-text-embeddings) ð¢ **Train/Infer Powerful Sentence Embeddings with
+AnglE.** This library is from the paper: [AnglE: Angle-optimized Text
+Embeddings](https://arxiv.org/abs/2309.12871). It allows for training state-of-
+the-art BERT/LLM-based sentence embeddings with just a few lines of code. AnglE
+is also a general sentence embedding inference framework, allowing for infering
+a variety of transformer-based sentence embeddings. ## â¨ Features **Loss**: -
+ð AnglE loss - â Contrastive loss - ð CoSENT loss - âï¸ Espresso
+loss (previously known as 2DMSE, detail: [README_ESE](README_ESE.md))
+**Backbones**: - BERT-based models (BERT, RoBERTa, ELECTRA, ALBERT, etc.) -
+LLM-based models (LLaMA, Mistral, Qwen, etc.) - Bi-directional LLM-based models
+(LLaMA, Mistral, Qwen, OpenELMo, etc.. refer to: https://github.com/WhereIsAI/
+BiLLM) **Training**: - Single-GPU training - Multi-GPU training > _[_h_t_t_p_:_/_/
+_m_a_k_e_a_p_u_l_l_r_e_q_u_e_s_t_._c_o_m_]More features will be added in the future. ## ð
+Achievements ð May 16, 2024 | Paper "[AnglE: Angle-optimized Text
+Embeddings](https://arxiv.org/abs/2309.12871)" is accepted by ACL 2024 Main
+Conference. ð Mar 13, 2024 | Paper "[BeLLM: Backward Dependency Enhanced
+Large Language Model for Sentence Embeddings](https://arxiv.org/abs/
+2311.05296)" is accepted by NAACL 2024 Main Conference. ð Mar 8, 2024 | ð
+[mixedbread's embedding](https://www.mixedbread.ai/blog/mxbai-embed-large-v1) (
+[mixedbread-ai/mxbai-embed-large-v1](https://huggingface.co/mixedbread-ai/
+mxbai-embed-large-v1)) achieves SOTA on the [MTEB Leaderboard](https://
+huggingface.co/spaces/mteb/leaderboard) with an average score of **64.68**! The
+model is trained using AnglE. Congrats mixedbread! ð Dec 4, 2023 | Our
+universal sentence embedding [WhereIsAI/UAE-Large-V1](https://huggingface.co/
+WhereIsAI/UAE-Large-V1) achieves SOTA on the [MTEB Leaderboard](https://
+huggingface.co/spaces/mteb/leaderboard) with an average score of **64.64**! The
+model is trained using AnglE. ð Dec, 2023 | AnglE achieves SOTA performance
+on the STS Bechmark Semantic Textual Similarity! ## ð¤ Official Pretrained
+Models BERT-based models: | ð¤ HF | Max Tokens | Pooling Strategy | Scenario
+| |----|------|------|------| | [WhereIsAI/UAE-Large-V1](https://
+huggingface.co/WhereIsAI/UAE-Large-V1) | 512 | cls | English, General-purpose |
+| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1)
+| 512 | cls | Code Similarity | LLM-based models: | ð¤ HF (lora weight) |
+Backbone | Max Tokens | Prompts | Pooling Strategy | Scenario | |----|------|--
+----|------|------|------| | [SeanLee97/angle-llama-13b-nli](https://
+huggingface.co/SeanLee97/angle-llama-13b-nli) | NousResearch/Llama-2-13b-hf |
+4096 | `Prompts.A` | last token | English, Similarity Measurement | |
 [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-
-7b-nli-v2) | Y | NousResearch/Llama-2-7b-hf | Y | EN | `Prompts.A` | last token
-| / | | [SeanLee97/angle-llama-7b-nli-20231027](https://huggingface.co/
-SeanLee97/angle-llama-7b-nli-20231027) | Y | NousResearch/Llama-2-7b-hf | Y |
-EN | `Prompts.A` | last token | / | | [SeanLee97/angle-bert-base-uncased-nli-
-en-v1](https://huggingface.co/SeanLee97/angle-bert-base-uncased-nli-en-v1) | N
-| N | N | EN | N | `cls_avg` | / | | [SeanLee97/angle-roberta-wwm-base-zhnli-
-v1](https://huggingface.co/SeanLee97/angle-roberta-wwm-base-zhnli-v1) | N | N |
-N | ZH-CN | N | `cls` | / | | [SeanLee97/angle-llama-7b-zhnli-v1](https://
-huggingface.co/SeanLee97/angle-llama-7b-zhnli-v1) | Y | NousResearch/Llama-2-
-7b-hf | Y | ZH-CN | `Prompts.B` | last token | / | ð¡ If the selected model
-is a LoRA weight, it must specify the corresponding dependent backbone. For our
-STS Experiment, please refer to https://github.com/SeanLee97/AnglE/tree/main/
-examples/NLI ## Results ### English STS Results | Model | STS12 | STS13 | STS14
-| STS15 | STS16 | STSBenchmark | SICKRelatedness | Avg. | | ------- |-------|--
------|-------|-------|-------|--------------|-----------------|-------| |
-[SeanLee97/angle-llama-7b-nli-20231027](https://huggingface.co/SeanLee97/angle-
-llama-7b-nli-20231027) | 78.68 | 90.58 | 85.49 | 89.56 | 86.91 | 88.92 | 81.18
-| 85.90 | | [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/
-angle-llama-7b-nli-v2) | 79.00 | 90.56 | 85.79 | 89.43 | 87.00 | 88.97 | 80.94
-| 85.96 | | [SeanLee97/angle-llama-13b-nli](https://huggingface.co/SeanLee97/
-angle-llama-13b-nli) | 79.33 | 90.65 | 86.89 | 90.45 | 87.32 | 89.69 | 81.32 |
-**86.52** | | [SeanLee97/angle-bert-base-uncased-nli-en-v1](https://
-huggingface.co/SeanLee97/angle-bert-base-uncased-nli-en-v1) | 75.09 | 85.56 |
-80.66 | 86.44 | 82.47 | 85.16 | 81.23 | 82.37 | ### Chinese STS Results | Model
-| ATEC | BQ | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc | Avg. | | ------- |---
-----|-------|-------|-------|-------|--------------|-----------------|-------
-| | ^[shibing624/text2vec-bge-large-chinese](https://huggingface.co/shibing624/
-text2vec-bge-large-chinese) | 38.41 | 61.34 | 71.72 | 35.15 | 76.44 | 71.81 |
-63.15 | 59.72 | | ^[shibing624/text2vec-base-chinese-paraphrase](https://
-huggingface.co/shibing624/text2vec-base-chinese-paraphrase) | 44.89 | 63.58 |
-74.24 | 40.90 | 78.93 | 76.70 | 63.30 | 63.08 | | [SeanLee97/angle-roberta-wwm-
-base-zhnli-v1](https://huggingface.co/SeanLee97/angle-roberta-wwm-base-zhnli-
-v1) | 49.49 | 72.47 | 78.33 | 59.13 | 77.14 | 72.36 | 60.53 | **67.06** | |
-[SeanLee97/angle-llama-7b-zhnli-v1](https://huggingface.co/SeanLee97/angle-
-llama-7b-zhnli-v1) | 50.44 | 71.95 | 78.90 | 56.57 | 81.11 | 68.11 | 52.02 |
-65.59 | ^ denotes baselines, their results are retrieved from: https://
-github.com/shibing624/text2vec ## Usage AnglE supports two APIs, one is the
-`transformers` API, the other is the `AnglE` API. If you want to use the
-`AnglE` API, please install AnglE first: ```bash python -m pip install -
-U angle-emb ``` ### UAE 1) For Retrieval Purposes For retrieval purposes,
-please use the prompt `Prompts.C`. ```python from angle_emb import AnglE,
-Prompts angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1',
-pooling_strategy='cls').cuda() angle.set_prompt(prompt=Prompts.C) vec =
-angle.encode({'text': 'hello world'}, to_numpy=True) print(vec) vecs =
-angle.encode([{'text': 'hello world1'}, {'text': 'hello world2'}],
-to_numpy=True) print(vecs) ``` 2) For non-Retrieval Purposes ```python from
-angle_emb import AnglE angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1',
-pooling_strategy='cls').cuda() vec = angle.encode('hello world', to_numpy=True)
-print(vec) vecs = angle.encode(['hello world1', 'hello world2'], to_numpy=True)
-print(vecs) ``` Difference between retrieval and non-retrieval sentence
-embeddings. [click to expand] In UAE, we use different approaches for retrieval
-and non-retrieval tasks, each serving a different purpose. **Retrieval tasks
-aim to find relevant documents, and as a result, the related documents may not
-have strict semantic similarities to each other.** For instance, when querying
-"How about ChatGPT?", the related documents are those that contain information
-related to "ChatGPT," such as "ChatGPT is amazing..." or "ChatGPT is bad....".
-Conversely, **non-retrieval tasks, such as semantic textual similarity, require
-sentences that are semantically similar.** For example, a sentence semantically
-similar to "How about ChatGPT?" could be "What is your opinion about ChatGPT?".
-To distinguish between these two types of tasks, we use different prompts. For
-retrieval tasks, we use the prompt "Represent this sentence for searching
-relevant passages: {text}" (Prompts.C in angle_emb). For non-retrieval tasks,
-we set the prompt to empty, i.e., just input your text without specifying a
-prompt. So, if your scenario is retrieval-related, it is highly recommended to
-set the prompt with angle.set_prompt(prompt=Prompts.C). If not, leave the
-prompt empty or use angle.set_prompt(prompt=None). ### Angle-LLaMA 1) AnglE
-```python from angle_emb import AnglE, Prompts angle = AnglE.from_pretrained
-('NousResearch/Llama-2-7b-hf', pretrained_lora_path='SeanLee97/angle-llama-7b-
-nli-v2') print('All predefined prompts:', Prompts.list_prompts())
-angle.set_prompt(prompt=Prompts.A) print('prompt:', angle.prompt) vec =
-angle.encode({'text': 'hello world'}, to_numpy=True) print(vec) vecs =
-angle.encode([{'text': 'hello world1'}, {'text': 'hello world2'}],
-to_numpy=True) print(vecs) ``` 2) transformers ```python from angle_emb import
-AnglE, Prompts from transformers import AutoModelForCausalLM, AutoTokenizer
-from peft import PeftModel, PeftConfig peft_model_id = 'SeanLee97/angle-llama-
-7b-nli-v2' config = PeftConfig.from_pretrained(peft_model_id) tokenizer =
-AutoTokenizer.from_pretrained(config.base_model_name_or_path) model =
-AutoModelForCausalLM.from_pretrained(config.base_model_name_or_path).bfloat16
-().cuda() model = PeftModel.from_pretrained(model, peft_model_id).cuda() def
-decorate_text(text: str): return Prompts.A.format(text=text) inputs = 'hello
-world!' tok = tokenizer([decorate_text(inputs)], return_tensors='pt') for k, v
-in tok.items(): tok[k] = v.cuda() vec = model(output_hidden_states=True,
-**tok).hidden_states[-1][:, -1].float().detach().cpu().numpy() print(vec) ```
-### Angle-BERT 1) AnglE ```python from angle_emb import AnglE angle =
-AnglE.from_pretrained('SeanLee97/angle-bert-base-uncased-nli-en-v1',
-pooling_strategy='cls_avg').cuda() vec = angle.encode('hello world',
-to_numpy=True) print(vec) vecs = angle.encode(['hello world1', 'hello world2'],
-to_numpy=True) print(vecs) ``` 2) transformers ```python import torch from
-transformers import AutoModel, AutoTokenizer model_id = 'SeanLee97/angle-bert-
-base-uncased-nli-en-v1' tokenizer = AutoTokenizer.from_pretrained(model_id)
-model = AutoModel.from_pretrained(model_id).cuda() inputs = 'hello world!' tok
-= tokenizer([inputs], return_tensors='pt') for k, v in tok.items(): tok[k] =
-v.cuda() hidden_state = model(**tok).last_hidden_state vec = (hidden_state[:,
-0] + torch.mean(hidden_state, dim=1)) / 2.0 print(vec) ``` ## Custom Train ###
-1. Data Prepation We support two dataset formats: 1) `DatasetFormats.A`: it is
-a pair format with three columns: `text1`, `text2`, and `label` (0/1). 2)
+7b-nli-v2) | NousResearch/Llama-2-7b-hf | 4096 | `Prompts.A` | last token |
+English, Similarity Measurement | ## ð Quick Start ### â¬ï¸ Installation
+```bash python -m pip install -U angle-emb ``` ### â Load BERT-based Model 1)
+**With Prompts**: You can specify a prompt with `prompt=YOUR_PROMPT` in
+`encode` method. If set a prompt, the inputs should be a list of dict or a
+single dict with key `text`, where `text` is the placeholder in the prompt for
+the input text. You can use other placeholder names. We provide a set of
+predefined prompts in `Prompts` class, you can check them via
+`Prompts.list_prompts()`. ```python from angle_emb import AnglE, Prompts from
+angle_emb.utils import cosine_similarity angle = AnglE.from_pretrained
+('WhereIsAI/UAE-Large-V1', pooling_strategy='cls').cuda() # For retrieval
+tasks, we use `Prompts.C` as the prompt for the query when using UAE-Large-V1
+(no need to specify prompt for documents). # When specify prompt, the inputs
+should be a list of dict with key 'text' qv = angle.encode({'text': 'what is
+the weather?'}, to_numpy=True, prompt=Prompts.C) doc_vecs = angle.encode([ 'The
+weather is great!', 'it is rainy today.', 'i am going to bed' ], to_numpy=True)
+for dv in doc_vecs: print(cosine_similarity(qv[0], dv)) ``` 2) **Without
+Prompts**: no need to specify a prompt. Just input a list of strings or a
+single string. ```python from angle_emb import AnglE from angle_emb.utils
+import cosine_similarity angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-
+V1', pooling_strategy='cls').cuda() # for non-retrieval tasks, we don't need to
+specify prompt when using UAE-Large-V1. doc_vecs = angle.encode([ 'The weather
+is great!', 'The weather is very good!', 'i am going to bed' ]) for i, dv1 in
+enumerate(doc_vecs): for dv2 in doc_vecs[i+1:]: print(cosine_similarity(dv1,
+dv2)) ``` ### â Load LLM-based Models If the pretrained weight is a LoRA-
+based model, you need to specify the backbone via `model_name_or_path` and
+specify the LoRA path via the `pretrained_lora_path` in `from_pretrained`
+method. ```python from angle_emb import AnglE, Prompts angle =
+AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
+pretrained_lora_path='SeanLee97/angle-llama-7b-nli-v2',
+pooling_strategy='last', is_llm=True, torch_dtype='float16') print('All
+predefined prompts:', Prompts.list_prompts()) vec = angle.encode({'text':
+'hello world'}, to_numpy=True, prompt=Prompts.A) print(vec) vecs = angle.encode
+([{'text': 'hello world1'}, {'text': 'hello world2'}], to_numpy=True,
+prompt=Prompts.A) print(vecs) ``` ### â Load Third-party Models You can load
+any transformer-based third-party models such as `mixedbread-ai/mxbai-embed-
+large-v1`, `sentence-transformers/all-MiniLM-L6-v2`, and `BAAI/bge-large-en-
+v1.5` using `angle_emb`. Here is an example: ```python from angle_emb import
+AnglE model = AnglE.from_pretrained('mixedbread-ai/mxbai-embed-large-v1',
+pooling_strategy='cls').cuda() vec = model.encode('hello world', to_numpy=True)
+print(vec) ``` ## ð¸ï¸ Custom Train ### ðï¸ 1. Data Prepation We
+currently support three dataset formats: 1) `DatasetFormats.A`: it is a pair
+format with three columns: `text1`, `text2`, and `label` (0/1). 2)
 `DatasetFormats.B`: it is a triple format with three columns: `text`,
 `positive`, and `negative`. `positive` and `negative` store the positive and
 negative samples of `text`. 3) `DatasetFormats.C`: it is a pair format with two
 columns: `text`, `positive`. `positive` store the positive sample of `text`.
 You need to prepare your data into huggingface `datasets.Dataset` in one of the
-formats in terms of your supervised data. ### 2. Train Use `angle-trainer` to
-train your AnglE model in cli mode. Usage: `CUDA_VISIBLE_DEVICES=0 angle-
-trainer --help` ### 3. Example [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/1h28jHvv_x-0fZ0tItIMjf8rJGp3GcO5V?usp=sharing)
-```python from datasets import load_dataset from angle_emb import AnglE,
-AngleDataTokenizer # 1. load pretrained model angle = AnglE.from_pretrained
-('SeanLee97/angle-bert-base-uncased-nli-en-v1', max_length=128,
-pooling_strategy='cls').cuda() # 2. load dataset # `text1`, `text2`, and
-`label` are three required columns. ds = load_dataset('mteb/stsbenchmark-sts')
-ds = ds.map(lambda obj: {"text1": str(obj["sentence1"]), "text2": str(obj
-['sentence2']), "label": obj['score']}) ds = ds.select_columns(["text1",
-"text2", "label"]) # 3. transform data train_ds = ds['train'].shuffle().map
-(AngleDataTokenizer(angle.tokenizer, angle.max_length), num_proc=8) valid_ds =
-ds['validation'].map(AngleDataTokenizer(angle.tokenizer, angle.max_length),
-num_proc=8) test_ds = ds['test'].map(AngleDataTokenizer(angle.tokenizer,
-angle.max_length), num_proc=8) # 4. fit angle.fit( train_ds=train_ds,
-valid_ds=valid_ds, output_dir='ckpts/sts-b', batch_size=32, epochs=5,
-learning_rate=2e-5, save_steps=100, eval_steps=1000, warmup_steps=0,
-gradient_accumulation_steps=1, loss_kwargs={ 'w1': 1.0, 'w2': 1.0, 'w3': 1.0,
-'cosine_tau': 20, 'ibn_tau': 20, 'angle_tau': 1.0 }, fp16=True,
-logging_steps=100 ) # 5. evaluate corrcoef, accuracy = angle.evaluate(test_ds,
-device=angle.device) print('corrcoef:', corrcoef) ``` # Citation You are
-welcome to use our code and pre-trained models. If you use our code and pre-
-trained models, please support us by citing our work as follows: ```bibtex
-@article{li2023angle, title={AnglE-optimized Text Embeddings}, author={Li,
-Xianming and Li, Jing}, journal={arXiv preprint arXiv:2309.12871}, year={2023}
-} ``` # ChangeLogs | ð | Description | |----|------| | 2024 Feb 7 | support
-training with only positive pairs (`DatasetFormats.C`) | | 2024 Jan 11 |
-refactor to support `angle-trainer` and BeLLM | | 2023 Dec 4 | Release a
-universal English sentence embedding model: [WhereIsAI/UAE-Large-V1](https://
-huggingface.co/WhereIsAI/UAE-Large-V1) | | 2023 Nov 2 | Release an English
-pretrained model: `SeanLee97/angle-llama-13b-nli` | | 2023 Oct 28 | Release two
-chinese pretrained models: `SeanLee97/angle-roberta-wwm-base-zhnli-v1` and
-`SeanLee97/angle-llama-7b-zhnli-v1`; Add chinese README.md |
+formats in terms of your supervised data. ### ð 2. Train with CLI Use
+`angle-trainer` to train your AnglE model in cli mode. 1) Single gpu training:
+Usage: ```bash CUDA_VISIBLE_DEVICES=0 angle-trainer --help ``` 2) Multi-gpu
+training: Usage: ```bash CUDA_VISIBLE_DEVICES=0,1 torchrun --nproc_per_node=2 -
+-master_port=1234 -m angle_emb.angle_trainer --help ``` ### ð 3. Custom
+Train [![Open In Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/drive/1h28jHvv_x-
+0fZ0tItIMjf8rJGp3GcO5V?usp=sharing) ```python from datasets import load_dataset
+from angle_emb import AnglE, AngleDataTokenizer # 1. load pretrained model
+angle = AnglE.from_pretrained('SeanLee97/angle-bert-base-uncased-nli-en-v1',
+max_length=128, pooling_strategy='cls').cuda() # 2. load dataset # `text1`,
+`text2`, and `label` are three required columns. ds = load_dataset('mteb/
+stsbenchmark-sts') ds = ds.map(lambda obj: {"text1": str(obj["sentence1"]),
+"text2": str(obj['sentence2']), "label": obj['score']}) ds = ds.select_columns(
+["text1", "text2", "label"]) # 3. transform data train_ds = ds['train'].shuffle
+().map(AngleDataTokenizer(angle.tokenizer, angle.max_length), num_proc=8)
+valid_ds = ds['validation'].map(AngleDataTokenizer(angle.tokenizer,
+angle.max_length), num_proc=8) test_ds = ds['test'].map(AngleDataTokenizer
+(angle.tokenizer, angle.max_length), num_proc=8) # 4. fit angle.fit
+( train_ds=train_ds, valid_ds=valid_ds, output_dir='ckpts/sts-b',
+batch_size=32, epochs=5, learning_rate=2e-5, save_steps=100, eval_steps=1000,
+warmup_steps=0, gradient_accumulation_steps=1, loss_kwargs={ 'cosine_w': 1.0,
+'ibn_w': 1.0, 'angle_w': 1.0, 'cosine_tau': 20, 'ibn_tau': 20, 'angle_tau': 20
+}, fp16=True, logging_steps=100 ) # 5. evaluate corrcoef, accuracy =
+angle.evaluate(test_ds, device=angle.device) print('corrcoef:', corrcoef) ```
+### ð¡ Others - To enable `llm` training, please specify `--is_llm 1` and
+configure appropriate LoRA hyperparameters. - To enable `billm` training,
+please specify `--apply_billm 1` and configure appropriate `billm_model_class`
+such as `LLamaForCausalLM` (refer to: https://github.com/WhereIsAI/
+BiLLM?tab=readme-ov-file#usage). - To enable espresso sentence embeddings
+(ESE), please specify `--apply_ese 1` and configure appropriate ESE
+hyperparameters via `--ese_kl_temperature float` and `--ese_compression_size
+integer`. - To convert the trained AnglE models to `sentence-transformers`,
+please run `python scripts/convert_to_sentence_transformers.py --help` for more
+details. ## ð¡ 4. Fine-tuning Tips 1ï¸â£ If your dataset format is
+`DatasetFormats.A`, it is recommended to slightly increase the weight for
+`cosine_w` or slightly decrease the weight for `ibn_w`. 2ï¸â£ If your dataset
+format is `DatasetFormats.B`, it is recommended to set `cosine_w` to 0, and
+increase the weight for `ibn_w` such as 10 and 20. The `angle_tau` is
+recommended to set to 20.0. 3ï¸â£ If your dataset format is
+`DatasetFormats.C`, only `ibn_w` and `ibn_tau` are effective. You don't need to
+tune other parameters. 4ï¸â£ To alleviate information forgetting in fine-
+tuning, it is better to specify the `teacher_name_or_path`. If the
+`teacher_name_or_path` equals `model_name_or_path`, it will conduct self-
+distillation. **It is worth to note that** `teacher_name_or_path` has to have
+the same tokenizer as `model_name_or_path`. Or it will lead to unexpected
+results. # ð«¡ Citation You are welcome to use our code and pre-trained
+models. If you use our code and pre-trained models, please support us by citing
+our work as follows: ```bibtex @article{li2023angle, title={AnglE-optimized
+Text Embeddings}, author={Li, Xianming and Li, Jing}, journal={arXiv preprint
+arXiv:2309.12871}, year={2023} } ``` # ð ChangeLogs | ð | Description |
+|----|------| | 2024 May 21 | support Espresso Sentence Embeddings | | 2024 Feb
+7 | support training with only positive pairs (`DatasetFormats.C`) | | 2023 Dec
+4 | Release a universal English sentence embedding model: [WhereIsAI/UAE-Large-
+V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) | | 2023 Nov 2 | Release an
+English pretrained model: `SeanLee97/angle-llama-13b-nli` | | 2023 Oct 28 |
+Release two chinese pretrained models: `SeanLee97/angle-roberta-wwm-base-zhnli-
+v1` and `SeanLee97/angle-llama-7b-zhnli-v1`; Add chinese README.md | # ð§
+Contact If you have any questions or suggestions, please feel free to contact
+us via email: xmlee97@gmail.com # Â© License This project is licensed under the
+MIT License. For the pretrained models, please refer to the corresponding
+license of the models.
```

### Comparing `angle_emb-0.3.9/angle_emb/angle.py` & `angle_emb-0.4.0/angle_emb/angle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import os
 import re
 import sys
 import json
 import copy
-import random
+import math
 from functools import partial
 from typing import Any, Dict, Optional, List, Union, Tuple, Callable
 from dataclasses import dataclass
 
 import scipy
 import scipy.stats
 import numpy as np
@@ -26,15 +26,14 @@
     TrainerCallback, BitsAndBytesConfig
 )
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.utils import PaddingStrategy
 from peft import (
     get_peft_model, LoraConfig, TaskType, PeftModel,
     prepare_model_for_kbit_training,
-    prepare_model_for_int8_training
 )
 from peft.tuners.lora import LoraLayer
 
 from .utils import logger
 
 
 DEFAULT_LLM_PATTERNS = [r'.*llama.*', r'.*qwen.*', r'.*baichuan.*', r'.*mistral.*']
@@ -110,15 +109,15 @@
     y_pred = y_pred[:, None] - y_pred[None, :]
     y_pred = (y_pred - (1 - y_true) * 1e12).view(-1)
     zero = torch.Tensor([0]).to(y_pred.device)
     y_pred = torch.concat((zero, y_pred), dim=0)
     return torch.logsumexp(y_pred, dim=0)
 
 
-def angle_loss(y_true: torch.Tensor, y_pred: torch.Tensor, tau: float = 1.0):
+def angle_loss(y_true: torch.Tensor, y_pred: torch.Tensor, tau: float = 1.0, pooling_strategy: str = 'sum'):
     """
     Compute angle loss
 
     :param y_true: torch.Tensor, ground truth.
         The y_true must be zigzag style, such as [x[0][0], x[0][1], x[1][0], x[1][1], ...], where (x[0][0], x[0][1]) stands for a pair.
     :param y_pred: torch.Tensor, model output.
         The y_pred must be zigzag style, such as [o[0][0], o[0][1], o[1][0], o[1][1], ...], where (o[0][0], o[0][1]) stands for a pair.
@@ -145,15 +144,21 @@
 
     dz = torch.sum(a**2 + b**2, dim=1, keepdim=True)**0.5
     dw = torch.sum(c**2 + d**2, dim=1, keepdim=True)**0.5
     re /= (dz / dw)
     im /= (dz / dw)
 
     y_pred = torch.concat((re, im), dim=1)
-    y_pred = torch.abs(torch.sum(y_pred, dim=1)) * tau  # absolute delta angle
+    if pooling_strategy == 'sum':
+        pooling = torch.sum(y_pred, dim=1)
+    elif pooling_strategy == 'mean':
+        pooling = torch.mean(y_pred, dim=1)
+    else:
+        raise ValueError(f'Unsupported pooling strategy: {pooling_strategy}')
+    y_pred = torch.abs(pooling) * tau  # absolute delta angle
     y_pred = y_pred[:, None] - y_pred[None, :]
     y_pred = (y_pred - (1 - y_true) * 1e12).view(-1)
     zero = torch.Tensor([0]).to(y_pred.device)
     y_pred = torch.concat((zero, y_pred), dim=0)
     return torch.logsumexp(y_pred, dim=0)
 
 
@@ -280,16 +285,15 @@
     return False
 
 
 def get_pooling(outputs: torch.Tensor,
                 inputs: Dict,
                 pooling_strategy: str,
                 padding_strategy: str = 'right') -> torch.Tensor:
-    """
-    get pooling
+    """ Pooling the model outputs.
 
     :param outputs:  torch.Tensor. Model outputs (without pooling)
     :param inputs:  Dict. Model inputs
     :param pooling_strategy:  str. Pooling strategy ['cls', 'cls_avg', 'cls_max', 'last', 'avg', 'max', 'all', index]
     :param padding_strategy:  str. Padding strategy of tokenizers (`left` or `right`).
         It can be obtained by `tokenizer.padding_side`.
     """
@@ -319,40 +323,26 @@
         outputs = outputs[:, int(pooling_strategy)]
     else:
         raise NotImplementedError(
             'please specify pooling_strategy from [`cls`, `last`, `avg`, `max`, `last_avg`, `all`, int]')
     return outputs
 
 
-def get_geometric_hidden_sizes(base: int = 8, max_hidden: int = 768) -> List[int]:
-    """
-    get geometric hidden size series list given a hidden size range
-
-    """
-    lst = []
-    s = base
-    while s < max_hidden:
-        lst.append(s)
-        s *= 2
-    return lst
-
-
 class Prompts:
     """
     Predefined prompts. Follow the model usage to choose the corresponding prompt.
 
     Example::
 
             from angle_emb import Prompts
 
             # list all pre-defined prompts
             print(Prompts.list_prompts())
             # set prompt
-            angle.set_prompt(prompt=Prompts.A)
-
+            angle.encode(*, prompt=Prompts.A)
     """
 
     A = 'Summarize sentence "{text}" in one word:"'
     B = 'You can only output one word. Summarize "{text}":"'
     C = 'Represent this sentence for searching relevant passages: {text}'
 
     @classmethod
@@ -587,14 +577,20 @@
     tokenizer: PreTrainedTokenizerBase
     padding: Union[bool, str, PaddingStrategy] = 'longest'
     max_length: Optional[int] = None
     return_tensors: str = "pt"
     filter_duplicate: bool = True
 
     def __call__(self, features: List[Dict], return_tensors: str = "pt") -> Dict[str, torch.Tensor]:
+        """ Collate function for AngleDataTokenizer.
+
+        :param features: List[Dict]. Tokenized data
+        :param return_tensors: str. Default "pt"
+        :return: Dict[str, torch.Tensor]. Collated data
+        """
         if return_tensors is None:
             return_tensors = self.return_tensors
         has_token_type_ids = "token_type_ids" in features[0]
         end_with_eos = features[0]['extra']['end_with_eos']
 
         new_features = []
         duplicate_set = set()
@@ -692,247 +688,329 @@
     :param pooling_strategy: Optional[str]. Currently support [`cls`, `last`, `avg`, `cls_avg`, `max`]. Default None.
     :param padding_strategy: Optional[str]. `left` or `right`. Default None.
     :param is_llm: bool. Default False
     """
     def __init__(self,
                  model: PreTrainedModel,
                  pooling_strategy: Optional[Union[int, str]] = None,
-                 padding_strategy: Optional[str] = None,
-                 is_llm: bool = False):
+                 padding_strategy: Optional[str] = None):
         self.model = model
         self.pooling_strategy = pooling_strategy
         self.padding_strategy = padding_strategy
-        self.is_llm = is_llm
 
-    def __call__(self, inputs: Dict, layer_index: int = -1, embedding_size: Optional[int] = None,
-                 return_all_layer_outputs: bool = False) -> torch.Tensor:
-        """
+    def __call__(self,
+                 inputs: Dict,
+                 layer_index: int = -1,
+                 embedding_start: Optional[int] = None,
+                 embedding_size: Optional[int] = None,
+                 return_all_layer_outputs: bool = False,
+                 pooling_strategy: Optional[Union[int, str]] = None,) -> torch.Tensor:
+        """ Get sentence embeddings.
         :param inputs: Dict. Model inputs.
-        :param layer_index: int. Get embeddings from specific layer.
-        :param embedding_size: int. Set embedding size for sentence embeddings for 2DMSE models.
+        :param layer_index: Optional[int]. Get embeddings from specific layer.
+        :param embedding_start: Optional[int]. Start index of embeddings.
+        :param embedding_size: int. Set embedding size for sentence embeddings.
+        :param return_all_layer_outputs: bool. Return all layer outputs or not. Default False.
+        :param pooling_strategy: Optional[str].
+            Currently support [`cls`, `last`, `avg`, `cls_avg`, `max`]. Default None.
         """
         all_layer_outputs = self.model(output_hidden_states=True, return_dict=True, **inputs).hidden_states
         if return_all_layer_outputs:
             return all_layer_outputs
         outputs = all_layer_outputs[layer_index]
-        if self.is_llm:
-            batch_size = inputs['input_ids'].shape[0]
-            sequence_lengths = -1 if self.padding_strategy == 'left' else inputs["attention_mask"].sum(dim=1) - 1
-            outputs = outputs[torch.arange(batch_size, device=outputs.device), sequence_lengths]
-        else:
-            outputs = get_pooling(outputs, inputs, self.pooling_strategy, padding_strategy=self.padding_strategy)
+        outputs = get_pooling(outputs, inputs,
+                              pooling_strategy or self.pooling_strategy,
+                              padding_strategy=self.padding_strategy)
+        n_dim = len(outputs.shape)
+        if embedding_start is not None:
+            if n_dim == 2:
+                outputs = outputs[:, embedding_start:]
+            elif n_dim == 3:
+                outputs = outputs[:, :, embedding_start:]
+            else:
+                raise ValueError(f'Unsupported output shape: {outputs.shape}')
         if embedding_size is not None:
             # topk embedding size
-            return outputs[:, :embedding_size]
+            if n_dim == 2:
+                outputs = outputs[:, :embedding_size]
+            elif n_dim == 3:
+                outputs = outputs[:, :, :embedding_size]
+            else:
+                raise ValueError(f'Unsupported output shape: {outputs.shape}')
         return outputs
 
 
 class AngleTrainer(Trainer):
     """
     Custom Huggingface Trainer for AnglE.
 
     :param pooler: Pooler. Required
     :param loss_kwargs: Optional[Dict]. Default None.
     :param dataset_format: str. Default DatasetFormats.A
-    :param fixed_teacher_name_or_path: Optional[str]. For distribution alignment.
+    :param teacher_name_or_path: Optional[str]. For distribution alignment.
     :param **kwargs: other parameters of Trainer.
     """
     def __init__(self,
                  pooler: Pooler,
                  loss_kwargs: Optional[Dict] = None,
                  dataset_format: str = DatasetFormats.A,
-                 fixed_teacher_name_or_path: Optional[str] = None,
-                 alignment_pooling_strategy: str = 'cls',
+                 teacher_name_or_path: Optional[str] = None,
+                 teacher_pooling_strategy: str = 'cls',
                  **kwargs):
         super().__init__(**kwargs)
         self.pooler = pooler
         if loss_kwargs is None:
             loss_kwargs = {}
         self.loss_fct = AngleLoss(dataset_format=dataset_format, **loss_kwargs)
-        self.fixed_teacher_name_or_path = fixed_teacher_name_or_path
-        self.alignment_pooling_strategy = alignment_pooling_strategy
-        if fixed_teacher_name_or_path is not None:
-            assert not check_llm(fixed_teacher_name_or_path), ('Currently not support LLMs alignment,'
-                                                               f' teacher={fixed_teacher_name_or_path}')
-            assert self.pooler.pooling_strategy == 'all', ('fixed_teacher_name_or_path detected!'
-                                                           ' please set --pooling_strategy all')
-            fixed_teacher_backbone = AutoModel.from_pretrained(
-                fixed_teacher_name_or_path,
+        self.teacher_name_or_path = teacher_name_or_path
+        self.teacher_pooling_strategy = teacher_pooling_strategy
+        if teacher_name_or_path is not None:
+            logger.info('Teacher detected! '
+                        'please ensure the teacher has the same tokenizer as the backbone model!')
+            assert not check_llm(teacher_name_or_path), ('Currently not support LLMs alignment,'
+                                                         f' teacher={teacher_name_or_path}')
+            teacher_backbone = AutoModel.from_pretrained(
+                teacher_name_or_path,
                 trust_remote_code=True,
-                torch_dtype="auto")
+                torch_dtype=self.pooler.model.dtype).to(self.pooler.model.device)
 
-            fixed_teacher_backbone.config.use_cache = False
-            self.fixed_teacher_pooler = Pooler(
-                fixed_teacher_backbone,
-                pooling_strategy='all',
-                padding_strategy=self.pooler.padding_strategy,
-                is_llm=False)
-            self.kl_loss_fct = nn.KLDivLoss(reduction='batchmean')
-            logger.info(f'Train with alignment, teacher={fixed_teacher_name_or_path}')
+            self.teacher_pooler = Pooler(
+                teacher_backbone,
+                pooling_strategy=self.teacher_pooling_strategy,
+                padding_strategy=self.pooler.padding_strategy)
+            logger.info(f'Train with teacher={teacher_name_or_path}')
+
+    def distillation_loss(self,
+                          inputs: torch.Tensor,
+                          targets: torch.Tensor,
+                          mse_weight: float = 1.0,
+                          kl_temperature: float = 1.0) -> torch.Tensor:
+        """ Compute distillation loss.
+
+        :param inputs: torch.Tensor. Input tensor.
+        :param targets: torch.Tensor. Target tensor.
+        :param mse_weight: float. MSE weight. Default 1.0.
+        :param kl_temperature: float. KL temperature. Default 1.0.
+        :return: torch.Tensor. Distillation loss.
+        """
+        loss = 0.
+        if mse_weight > 0:
+            loss += mse_weight * nn.MSELoss()(inputs, targets)
+        if kl_temperature > 0:
+            loss += nn.KLDivLoss(reduction='batchmean')(
+                F.log_softmax(inputs / kl_temperature, dim=-1),
+                F.softmax(targets / kl_temperature, dim=-1)
+            ) * kl_temperature
+        return loss
 
     def compute_loss(self, model, inputs, return_outputs=False):
+        """ Compute loss for AnglE.
+
+        :param model: Huggingface model.
+        :param inputs: Dict. Model inputs.
+        :param return_outputs: bool. Return outputs or not. Default False.
+        :return: torch.Tensor. Loss.
+        """
         labels = inputs.pop("labels", None)
-        if self.fixed_teacher_name_or_path is not None:
-            all_outputs = self.pooler(inputs)
+        if self.teacher_name_or_path is not None:
+            all_outputs = self.pooler(inputs, layer_index=-1, return_all_layer_outputs=True)[-1]
             outputs = get_pooling(all_outputs, inputs,
-                                  self.alignment_pooling_strategy,
+                                  self.pooler.pooling_strategy,
                                   self.pooler.padding_strategy)
             loss = self.loss_fct(labels, outputs)
             with torch.no_grad():
-                self.fixed_teacher_pooler.model = self.fixed_teacher_pooler.model.to(self.pooler.model.device)
-                all_fixed_outputs = self.fixed_teacher_pooler(inputs)
+                self.teacher_pooler.model = self.teacher_pooler.model.to(self.pooler.model.device)
+                align_outputs = self.teacher_pooler(inputs)
 
-            alignment_loss = self.kl_loss_fct(
-                F.log_softmax(all_outputs, dim=-1),
-                F.softmax(all_fixed_outputs, dim=-1)
-            )
+            alignment_loss = self.distillation_loss(
+                all_outputs if self.teacher_pooling_strategy == 'all' else outputs,
+                align_outputs,
+                mse_weight=0.0,
+                kl_temperature=1.0)
             loss += alignment_loss
         else:
             outputs = self.pooler(inputs)
             loss = self.loss_fct(labels, outputs)
 
         return (loss, outputs) if return_outputs else loss
 
 
-class AngleTDMSETrainer(AngleTrainer):
+class AngleESETrainer(AngleTrainer):
     """
-    Custom Huggingface Trainer for AnglE 2DMSE.
+    Custom Huggingface Trainer for AnglE Espresso.
 
     :param pooler: Pooler. Required
     :param loss_kwargs: Optional[Dict]. Default None.
     :param dataset_format: str. Default DatasetFormats.A
-    :param fixed_teacher_name_or_path: Optional[str]. For distribution alignment.
+    :param teacher_name_or_path: Optional[str]. For distribution alignment.
 
     :param **kwargs: other parameters of Trainer.
     """
     def __init__(self,
                  pooler: Pooler,
                  loss_kwargs: Optional[Dict] = None,
                  dataset_format: str = DatasetFormats.A,
-                 fixed_teacher_name_or_path: Optional[str] = None,
-                 tdmse_kl_temperature: float = 1.0,
-                 tdmse_teacher_lambda: float = 1.0,
-                 tdmse_student_lambda: float = 1.0,
-                 apply_tdmse_kl: bool = True,
+                 teacher_name_or_path: Optional[str] = None,
+                 ese_kl_temperature: float = 1.0,
+                 ese_compression_size: int = 128,
+                 apply_ese_pca: bool = True,
                  **kwargs):
         super().__init__(pooler=pooler,
                          loss_kwargs=loss_kwargs,
                          dataset_format=dataset_format,
-                         fixed_teacher_name_or_path=fixed_teacher_name_or_path,
+                         teacher_name_or_path=teacher_name_or_path,
                          **kwargs)
-        self.tdmse_kl_temperature = tdmse_kl_temperature
-        self.tdmse_teacher_lambda = tdmse_teacher_lambda
-        self.tdmse_student_lambda = tdmse_student_lambda
-        self.apply_tdmse_kl = apply_tdmse_kl
+        self.ese_kl_temperature = ese_kl_temperature
+        self.ese_compression_size = ese_compression_size
+        self.apply_ese_pca = apply_ese_pca
         self.n_layers = self.pooler.model.config.num_hidden_layers
-        self.hidden_size = self.pooler.model.config.hidden_size
-        self.tdmse_hidden_sizes = get_geometric_hidden_sizes(base=8, max_hidden=self.hidden_size)
-        self.kl_loss_fct = nn.KLDivLoss(reduction='batchmean')
-        logger.info('Train with 2DMSE!')
+        logger.info('Train with ☕️ Espresso!')
+
+    @torch.no_grad()
+    def pca_compress(self, m: torch.Tensor, k: int) -> torch.Tensor:
+        """ Get topk feature via PCA.
+        :param m: torch.Tensor. Input tensor.
+        :param k: int. Top-k feature size.
+        :return: torch.Tensor. Top-k feature.
+        """
+        A = F.softmax(m.T @ m / m.shape[-1]**0.5, dim=-1)
+        u, s, _ = torch.svd_lowrank(A, q=k)
+        # top-k principal components
+        topk_deps = u @ torch.diag(s)
+        return m @ topk_deps
+
+    def compute_student_loss(self,
+                             inputs: Dict,
+                             all_layer_outputs: torch.Tensor,
+                             labels: torch.Tensor,
+                             pooling_strategy: str,
+                             padding_strategy: str) -> torch.Tensor:
+        loss = 0.
+        compression_loss = 0.
+        for i in range(self.n_layers - 1):
+            division = (1. + math.log(1 + i))
+            all_student_outputs = all_layer_outputs[i]
+            student_outputs = get_pooling(all_student_outputs,
+                                          inputs,
+                                          pooling_strategy,
+                                          padding_strategy)
+
+            slimmed_outputs = student_outputs[:, :self.ese_compression_size]
+            loss += self.loss_fct(labels, slimmed_outputs) / division
+            if self.apply_ese_pca:
+                compression_loss += self.distillation_loss(
+                    slimmed_outputs,
+                    self.pca_compress(student_outputs, self.ese_compression_size),
+                    kl_temperature=self.ese_kl_temperature
+                ) / division
+        return (loss + compression_loss) / (self.n_layers - 1)
 
     def compute_loss(self, model, inputs, return_outputs=False):
+        """ Compute loss for Espresso.
+        :param model: Huggingface model.
+        :param inputs: Dict. Model inputs.
+        :param return_outputs: bool. Return outputs or not. Default False.
+        :return: torch.Tensor. Loss.
+        """
         labels = inputs.pop("labels", None)
         # layer
-        sample_layer = random.randint(1, self.n_layers - 1)
-        pooling_strategy = (self.alignment_pooling_strategy
-                            if self.pooler.pooling_strategy == 'all'
-                            else self.pooler.pooling_strategy)
         all_layer_outputs = self.pooler(inputs, layer_index=-1, return_all_layer_outputs=True)
         all_teacher_outputs = all_layer_outputs[-1]
         teacher_outputs = get_pooling(all_teacher_outputs, inputs,
-                                      pooling_strategy,
-                                      self.pooler.padding_strategy)
-        all_student_outputs = all_layer_outputs[sample_layer]
-        student_outputs = get_pooling(all_student_outputs,
-                                      inputs,
-                                      pooling_strategy,
+                                      self.pooler.pooling_strategy,
                                       self.pooler.padding_strategy)
 
-        teacher_kl_outputs = teacher_outputs
-        if self.fixed_teacher_name_or_path is not None:
-            with torch.no_grad():
-                self.fixed_teacher_pooler.model = self.fixed_teacher_pooler.model.to(self.pooler.model.device)
-                all_fixed_outputs = self.fixed_teacher_pooler(inputs)
-                teacher_kl_outputs = get_pooling(all_fixed_outputs,
-                                                 inputs,
-                                                 self.alignment_pooling_strategy,
-                                                 self.pooler.padding_strategy)
-
-        teacher_loss = self.loss_fct(labels, teacher_outputs)
-        loss1 = teacher_loss
-        student_loss = self.loss_fct(labels, student_outputs)
-        loss1 += student_loss / sample_layer
-        if self.apply_tdmse_kl and self.tdmse_student_lambda > 0:
-            kl_loss = self.kl_loss_fct(
-                F.log_softmax(student_outputs / self.tdmse_kl_temperature, dim=-1),
-                F.softmax(teacher_kl_outputs / self.tdmse_kl_temperature, dim=-1)
-            ) * self.tdmse_kl_temperature
-            loss1 += kl_loss
-
-        # feature
-        hidden_size = random.choice(self.tdmse_hidden_sizes)
-        slimmed_teacher_outputs = teacher_outputs[:, :hidden_size]
-        slimmed_student_outputs = student_outputs[:, :hidden_size]
-
-        slimmed_teacher_loss = self.loss_fct(labels, slimmed_teacher_outputs)
-        loss2 = slimmed_teacher_loss
-        slimmed_student_loss = self.loss_fct(labels, slimmed_student_outputs)
-        loss2 += slimmed_student_loss / sample_layer
-
-        loss = loss1 + loss2
-
-        if self.fixed_teacher_name_or_path is not None:
-            alignment_loss = self.kl_loss_fct(
-                F.log_softmax(all_teacher_outputs, dim=-1),
-                F.softmax(all_fixed_outputs, dim=-1)
+        loss = self.loss_fct(labels, teacher_outputs)
+
+        slimmed_outputs = teacher_outputs[:, :self.ese_compression_size]
+        loss += self.loss_fct(labels, slimmed_outputs)
+        if self.apply_ese_pca:
+            loss += self.distillation_loss(
+                slimmed_outputs,
+                self.pca_compress(teacher_outputs, self.ese_compression_size),
+                kl_temperature=self.ese_kl_temperature
             )
-            loss += alignment_loss
+
+        # student loss
+        loss += self.compute_student_loss(
+            inputs,
+            all_layer_outputs,
+            labels,
+            self.pooler.pooling_strategy,
+            self.pooler.padding_strategy,
+        )
+
+        # alignment loss
+        if self.teacher_name_or_path is not None:
+            with torch.no_grad():
+                self.teacher_pooler.model = self.teacher_pooler.model.to(self.pooler.model.device)
+                align_outputs = self.teacher_pooler(inputs)
+                alignment_loss = self.distillation_loss(
+                    all_teacher_outputs if self.teacher_pooling_strategy == 'all' else teacher_outputs,
+                    align_outputs,
+                    mse_weight=0.0,
+                    kl_temperature=1.0
+                )
+                loss += alignment_loss
         return (loss, teacher_outputs) if return_outputs else loss
 
 
 class AngleLoss:
     """
     Configure AngleLoss.
 
-    :param w1: float. weight for cosine_loss. Default 1.0
-    :param w2: float. weight for contrastive loss. Default 1.0
-    :param w3: float. weight for angle loss. Default 1.0
+    :param cosine_w: float. weight for cosine_loss. Default 1.0
+    :param ibn_w: float. weight for contrastive loss. Default 1.0
+    :param angle_w: float. weight for angle loss. Default 1.0
     :param cosine_tau: float. tau for cosine loss. Default 20.0
     :param ibn_tau: float. tau for contrastive loss. Default 20.0
-    :param angle_tau: float. tau for angle loss. Default 1.0
+    :param angle_tau: float. tau for angle loss. Default 20.0
+    :param angle_pooling_strategy: str. pooling strategy for angle loss. Default'sum'.
     :param dataset_format: Optional[str]. Default None.
     """
     def __init__(self,
-                 w1: float = 1.0,
-                 w2: float = 1.0,
-                 w3: float = 1.0,
+                 cosine_w: float = 1.0,
+                 ibn_w: float = 1.0,
+                 angle_w: float = 1.0,
                  cosine_tau: float = 20.0,
                  ibn_tau: float = 20.0,
-                 angle_tau: float = 1.0,
+                 angle_tau: float = 20.0,
+                 angle_pooling_strategy: str = 'sum',
                  dataset_format: Optional[str] = None,
                  **kwargs):
-        self.w1 = w1
-        self.w2 = w2
-        self.w3 = w3
+        if 'w1' in kwargs or 'w2' in kwargs or 'w3' in kwargs:
+            assert ('w1, w2, and w3 has been renamed to cosine_w, ibn_w, and angle_w, respecitvely.'
+                    'Please use new names instead.')
+        self.cosine_w = cosine_w
+        self.ibn_w = ibn_w
+        self.angle_w = angle_w
         self.cosine_tau = cosine_tau
         self.ibn_tau = ibn_tau
         self.angle_tau = angle_tau
+        self.angle_pooling_strategy = angle_pooling_strategy
         self.dataset_format = dataset_format
 
     def __call__(self,
                  labels: torch.Tensor,
                  outputs: torch.Tensor) -> torch.Tensor:
+        """ Compute loss for AnglE.
+
+        :param labels: torch.Tensor. Labels.
+        :param outputs: torch.Tensor. Outputs.
+        :return: torch.Tensor. Loss.
+        """
         if self.dataset_format == DatasetFormats.A:
             loss = 0.
-            if self.w1 > 0:
-                loss += self.w1 * cosine_loss(labels, outputs, self.cosine_tau)
-            if self.w2 > 0:
-                loss += self.w2 * in_batch_negative_loss(labels, outputs, self.ibn_tau)
-            if self.w3 > 0:
-                loss += self.w3 * angle_loss(labels, outputs, self.angle_tau)
+            if self.cosine_w > 0:
+                loss += self.cosine_w * cosine_loss(labels, outputs, self.cosine_tau)
+            if self.ibn_w > 0:
+                loss += self.ibn_w * in_batch_negative_loss(labels, outputs, self.ibn_tau)
+            if self.angle_w > 0:
+                loss += self.angle_w * angle_loss(labels, outputs, self.angle_tau,
+                                                  pooling_strategy=self.angle_pooling_strategy)
         elif self.dataset_format == DatasetFormats.B:
             # text,positive,negative
             text = outputs[::3]
             positive = outputs[1::3]
             negative = outputs[2::3]
             assert text.shape == positive.shape == negative.shape, f'text.shape={text.shape}, postive.shape={positive.shape}, negative.shape={negative.shape}'  # NOQA
 
@@ -941,20 +1019,21 @@
             positive_labels = torch.ones_like(positive_inputs[:, :1]).long()
             negative_inputs = torch.stack((text, negative), dim=1).reshape(-1, fea_dim)  # zip(text, negative)
             negative_labels = torch.zeros_like(negative_inputs[:, :1]).long()
             combined_inputs = torch.cat((positive_inputs, negative_inputs), dim=0)
             combined_labels = torch.cat((positive_labels, negative_labels), dim=0)
 
             loss = 0.
-            if self.w1 > 0:
-                loss += self.w1 * cosine_loss(combined_labels, combined_inputs, self.cosine_tau)
-            if self.w2 > 0:
-                loss += self.w2 * contrastive_with_negative_loss(text, positive, negative, tau=self.ibn_tau)
-            if self.w3 > 0:
-                loss += self.w3 * angle_loss(combined_labels, combined_inputs, self.angle_tau)
+            if self.cosine_w > 0:
+                loss += self.cosine_w * cosine_loss(combined_labels, combined_inputs, self.cosine_tau)
+            if self.ibn_w > 0:
+                loss += self.ibn_w * contrastive_with_negative_loss(text, positive, negative, tau=self.ibn_tau)
+            if self.angle_w > 0:
+                loss += self.angle_w * angle_loss(combined_labels, combined_inputs, self.angle_tau,
+                                                  pooling_strategy=self.angle_pooling_strategy)
         elif self.dataset_format == DatasetFormats.C:
             text = outputs[::2]
             positive = outputs[1::2]
             loss = contrastive_with_negative_loss(text, positive, neg=None, tau=self.ibn_tau)
         else:
             raise NotImplementedError
         return loss
@@ -1011,14 +1090,15 @@
     :param pretrained_model_path: Optional[str]. Default None.
     :param pretrained_lora_path: Optional[str]. Default None.
     :param apply_bfloat16: Optional[bool]. Whether load using torch.bfloat16. Default None.
     :param torch_dtype: Optional[torch.dtype]. Specify torch_dtype. Default None.
     :param device: Optional[str]. Specify device. Default None.
     :param kbit_kwargs: Optional[Dict]. kwargs for kbit. Default None.
         details refer to: https://huggingface.co/docs/peft/package_reference/peft_model#peft.prepare_model_for_kbit_training
+    :param tokenizer_padding_side: Optional[str]. Specify tokenizer padding side from [`left`, `right`]. Default None.
     :param **kwargs: Any.
     """  # NOQA
     cfg_file_name = 'angle.config'
 
     def __init__(self,
                  model_name_or_path: str,
                  max_length: int = 512,
@@ -1031,14 +1111,17 @@
                  is_llm: Optional[bool] = None,
                  pretrained_model_path: Optional[str] = None,
                  pretrained_lora_path: Optional[str] = None,
                  apply_bfloat16: Optional[bool] = None,
                  torch_dtype: Optional[torch.dtype] = None,
                  device: Optional[str] = None,
                  kbit_kwargs: Optional[Dict] = None,
+                 tokenizer_padding_side: Optional[str] = None,
+                 apply_billm: bool = False,
+                 billm_model_class: Optional[str] = None,
                  **kwargs: Any):
         super().__init__()
         self.max_length = max_length
         self.train_mode = train_mode
         self.pooling_strategy = pooling_strategy
         self.load_kbit = load_kbit
         self.is_llm = is_llm
@@ -1047,33 +1130,31 @@
         else:
             self.device = set_device()
         if is_llm is None:
             self.is_llm = check_llm(model_name_or_path)
             if self.is_llm:
                 logger.info('LLM detected, automatically set is_llm=True.'
                             'If it is wrong, you can manually set `is_llm`.')
+        if self.is_llm and self.pooling_strategy != 'last':
+            logger.info(f'🚨 LLM detected, but pooling strategy is specified to {self.pooling_strategy}.'
+                        'Please check whether it is correct. It is recommended to use `last` pooling strategy for LLM.')
+
         self.apply_lora = apply_lora
         if self.apply_lora is None:
             if self.is_llm:
                 self.apply_lora = True
                 logger.info('LLM detected, automatically set apply_lora=True.'
                             'If it is wrong, you can manually set `apply_lora`.')
         if self.device == 'cuda':
             self.gpu_count = torch.cuda.device_count()
         elif self.device == 'mps':
             self.gpu_count = 1
         else:
             self.gpu_count = 0
 
-        self.prompt = None
-        if self.is_llm:
-            logger.info('LLM detected, automatically set prompt. '
-                        'You can change this setting by manually configuring the `set_prompt()` function.')
-            self.set_prompt()
-
         self.apply_bfloat16 = apply_bfloat16
         if self.apply_bfloat16 is None and 'llama' in model_name_or_path.lower():
             logger.info('LLaMA detected, automatically set `apply_bfloat16=True`. '
                         'You can change this setting by manually configuring the `apply_bfloat16`.')
             self.apply_bfloat16 = True
 
         if torch_dtype is None:
@@ -1089,36 +1170,49 @@
             }
             if lora_config_kwargs is not None:
                 lora_config.update(lora_config_kwargs)
             if train_mode:
                 logger.info(f'lora_config={lora_config}')
 
         self.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path, trust_remote_code=True)
+        if tokenizer_padding_side is not None and self.tokenizer.padding_side != tokenizer_padding_side:
+            self.tokenizer.padding_side = tokenizer_padding_side
         if self.is_llm and self.tokenizer.pad_token_id is None:
             self.tokenizer.pad_token_id = 0
 
         model_kwargs = model_kwargs if model_kwargs is not None else {}
         kbit_kwargs = kbit_kwargs if kbit_kwargs is not None else {}
         if self.is_llm:
             device_map = "auto"
-            MODEL_CLASS = AutoModelForCausalLM
+            if apply_billm:
+                assert billm_model_class is not None, "billm_model_class should be specified for apply_billm=True"
+                try:
+                    import billm
+                except ImportError as err:
+                    print(f'Import Error: {err}')
+                    print('Please install the latest billm via: python -m pip install -U billm')
+                    raise
+
+                MODEL_CLASS = getattr(billm, billm_model_class)
+            else:
+                MODEL_CLASS = AutoModelForCausalLM
             if train_mode and self.gpu_count > 1:
                 device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
             # LLM
             if self.apply_lora:
                 lora_config['bias'] = "none"
                 lora_config['task_type'] = TaskType.CAUSAL_LM
 
-                if load_kbit == 4:
+                if load_kbit in [4, 8]:
                     model = MODEL_CLASS.from_pretrained(
                         model_name_or_path,
-                        load_in_4bit=True,
                         config=None,
                         quantization_config=BitsAndBytesConfig(
-                            load_in_4bit=True,
+                            load_in_4bit=load_kbit == 4,
+                            load_in_8bit=load_kbit == 8,
                             llm_int8_threshold=6.0,
                             llm_int8_has_fp16_weight=False,
                             bnb_4bit_compute_dtype=torch.float32,
                             bnb_4bit_use_double_quant=True,
                             bnb_4bit_quant_type='nf4',
                         ),
                         torch_dtype=torch.float32,
@@ -1134,81 +1228,64 @@
                             pretrained_lora_path,
                             torch_dtype=torch.float32,
                             device_map=device_map,
                             is_trainable=train_mode
                         )
                     elif train_mode:
                         if 'target_modules' not in lora_config or lora_config.get('target_modules', None) is None:
-                            target_modules = find_all_linear_names(model, linear_type=bnb.nn.Linear4bit)
+                            target_modules = find_all_linear_names(
+                                model, linear_type=bnb.nn.Linear4bit if load_kbit == 4 else nn.Linear)
                             lora_config['target_modules'] = target_modules
                             logger.info(f'lora target modules={target_modules}')
                         peft_config = LoraConfig(**lora_config)
                         model = get_peft_model(model, peft_config)
                     model = AnglE.kbit_post_handle(model)
                     self.backbone = model
                 else:
-                    if train_mode:
-                        model = MODEL_CLASS.from_pretrained(
-                            model_name_or_path,
-                            load_in_8bit=load_kbit == 8,
+                    if self.apply_bfloat16:
+                        model = MODEL_CLASS.from_pretrained(model_name_or_path,
+                                                            output_hidden_states=True,
+                                                            trust_remote_code=True).bfloat16()
+                    else:
+                        model = MODEL_CLASS.from_pretrained(model_name_or_path,
+                                                            device_map=device_map,
+                                                            output_hidden_states=True,
+                                                            trust_remote_code=True,
+                                                            torch_dtype=torch_dtype or torch.float16)
+
+                    if 'target_modules' not in lora_config or lora_config.get('target_modules', None) is None:
+                        target_modules = find_all_linear_names(model)
+                        lora_config['target_modules'] = target_modules
+                        logger.info(f'lora target modules={target_modules}')
+
+                    if pretrained_lora_path is not None:
+                        print(f'Load lora weight from {pretrained_lora_path}')
+                        model = PeftModel.from_pretrained(
+                            model,
+                            pretrained_lora_path,
                             torch_dtype=torch.float16 if load_kbit == 16 else torch.float32,
                             device_map=device_map,
-                            trust_remote_code=True,
+                            is_trainable=train_mode
                         )
-                        if load_kbit == 8:
-                            model = prepare_model_for_int8_training(model, **kbit_kwargs)
-                            if 'target_modules' not in lora_config or lora_config.get('target_modules', None) is None:
-                                target_modules = find_all_linear_names(model)
-                                lora_config['target_modules'] = target_modules
-                                logger.info(f'lora target modules={target_modules}')
-                        if pretrained_lora_path is not None:
-                            print(f'Load lora weight from {pretrained_lora_path}')
-                            model = PeftModel.from_pretrained(
-                                model,
-                                pretrained_lora_path,
-                                torch_dtype=torch.float16 if load_kbit == 16 else torch.float32,
-                                device_map=device_map,
-                                is_trainable=train_mode
-                            )
-                        else:
+                    else:
+                        if train_mode:
                             peft_config = LoraConfig(**lora_config)
                             model = get_peft_model(model, peft_config)
-                    else:
-                        if self.apply_bfloat16:
-                            model = MODEL_CLASS.from_pretrained(model_name_or_path,
-                                                                output_hidden_states=True,
-                                                                trust_remote_code=True).bfloat16()
-                        else:
-                            model = MODEL_CLASS.from_pretrained(model_name_or_path,
-                                                                device_map=device_map,
-                                                                output_hidden_states=True,
-                                                                trust_remote_code=True,
-                                                                load_in_8bit=load_kbit == 8,
-                                                                torch_dtype=torch_dtype or torch.float16)
-                        if pretrained_lora_path is not None:
-                            logger.info(f'Load lora weight from {pretrained_lora_path}')
-                            model = PeftModel.from_pretrained(
-                                model,
-                                pretrained_lora_path,
-                                torch_dtype=torch_dtype or torch.float16,
-                                device_map=device_map,
-                                is_trainable=train_mode
-                            )
+
                     self.backbone = model
             else:
                 if self.apply_bfloat16:
                     model = MODEL_CLASS.from_pretrained(model_name_or_path,
                                                         output_hidden_states=True,
                                                         trust_remote_code=True).bfloat16()
                 else:
                     model = MODEL_CLASS.from_pretrained(model_name_or_path,
                                                         device_map=device_map,
                                                         output_hidden_states=True,
                                                         trust_remote_code=True,
-                                                        load_in_8bit=load_kbit == 8,
                                                         torch_dtype=torch_dtype or torch.float16)
                 self.backbone = model
         else:
             # non-LLMs
             if self.apply_lora:
                 model = AutoModel.from_pretrained(pretrained_model_path or model_name_or_path, trust_remote_code=True)
                 if pretrained_lora_path is not None:
@@ -1236,26 +1313,29 @@
         if train_mode and self.apply_lora:
             self.backbone.print_trainable_parameters()
 
         self.backbone.config.use_cache = False
         self.pooler = Pooler(
             self.backbone,
             pooling_strategy=self.pooling_strategy,
-            padding_strategy=self.tokenizer.padding_side,
-            is_llm=self.is_llm)
+            padding_strategy=self.tokenizer.padding_side)
 
-        # full_backbone is used to 2DMSE inference
+        # full_backbone is used to Espresso inference
         self.full_backbone = None
         self.__cfg = {
             'model_name_or_path': model_name_or_path,
             'max_length': max_length,
             'model_kwargs': model_kwargs,
             'pooling_strategy': pooling_strategy,
             'lora_config_kwargs': lora_config,
-            'apply_lora': apply_lora,
+            'is_llm': self.is_llm,
+            'apply_billm': apply_billm,
+            'billm_model_class': billm_model_class,
+            'apply_lora': self.apply_lora,
+            'tokenizer_padding_side': tokenizer_padding_side,
         }
         self.__cfg.update(kwargs)
 
     def cuda(self):
         if self.load_kbit is None:
             self.backbone = self.backbone.to(torch.device(self.device))
         return self
@@ -1359,16 +1439,19 @@
             save_strategy: str = 'steps',
             save_total_limit: int = 10,
             gradient_accumulation_steps: int = 1,
             fp16: Optional[bool] = None,
             argument_kwargs: Optional[Dict] = None,
             trainer_kwargs: Optional[Dict] = None,
             loss_kwargs: Optional[Dict] = None,
-            apply_tdmse: bool = False,
-            filter_duplicate: bool = True):
+            apply_ese: bool = False,
+            filter_duplicate: bool = True,
+            push_to_hub: bool = False,
+            hub_model_id: Optional[str] = None,
+            hub_private_repo: bool = True):
         """
         Fit using AnglE.
 
         :param train_ds: Dataset. tokenized train dataset. Required.
         :param valid_ds: Optional[Dataset]. tokenized valid dataset. Default None.
         :param batch_size: int. Default 32.
         :param output_dir: Optional[str]. save dir. Default None.
@@ -1382,42 +1465,63 @@
         :param save_total_limit: int. Default 10.
         :param gradient_accumulation_steps: int. Default 1.
         :param fp16: Optional[bool]. Default None.
         :param argument_kwargs: Optional[Dict]. kwargs for TrainingArguments.
             refer to: https://huggingface.co/docs/transformers/v4.37.0/en/main_classes/trainer#transformers.TrainingArguments
         :param trainer_kwargs: Optional[Dict]. kwargs for AngleTrainer.
         :param loss_kwargs: Optional[Dict]. kwargs for AngleLoss.
-        :param apply_tdmse: bool, whether apply TDMSE training.
+        :param apply_ese: bool, whether apply ESE training.
+        :param filter_duplicate: bool, whether filter duplicate samples.
+        :param push_to_hub: bool, whether push to hub.
+        :param hub_model_id: Optional[str], hub model id.
+        :param hub_private_repo: bool, whether push to private repo.
         """  # NOQA
         if output_dir is not None:
             os.makedirs(output_dir, exist_ok=True)
         # save config
         self.save_config(os.path.join(output_dir, AnglE.cfg_file_name))
+        # save tokenizer
+        self.tokenizer.save_pretrained(output_dir)
 
         if self.gpu_count > 1:
             gradient_accumulation_steps = gradient_accumulation_steps // self.gpu_count
         if fp16 is None and self.is_llm:
             fp16 = True
         else:
             fp16 = False
+
+        # init argument_kwargs
         if argument_kwargs is None:
             argument_kwargs = {}
+        if 'push_to_hub' not in argument_kwargs:
+            argument_kwargs['push_to_hub'] = push_to_hub
+        if 'hub_model_id' not in argument_kwargs:
+            argument_kwargs['hub_model_id'] = hub_model_id
+        if 'hub_private_repo' not in argument_kwargs:
+            argument_kwargs['hub_private_repo'] = hub_private_repo
+
         if trainer_kwargs is None:
             trainer_kwargs = {}
+
         callbacks = None
         if valid_ds is not None:
+            # check format
+            for obj in valid_ds:
+                if obj['extra']['dataset_format'] != DatasetFormats.A:
+                    raise ValueError('Currently only support evaluation for DatasetFormats.A.')
+                break
             best_ckpt_dir = None
             if output_dir is not None:
                 best_ckpt_dir = os.path.join(output_dir, 'best-checkpoint')
             evaluate_callback = EvaluateCallback(self.backbone, valid_ds,
                                                  partial(self.evaluate, batch_size=batch_size, device=self.device),
                                                  save_dir=best_ckpt_dir)
             callbacks = [evaluate_callback]
 
-        CustomTrainer = AngleTDMSETrainer if apply_tdmse else AngleTrainer
+        CustomTrainer = AngleESETrainer if apply_ese else AngleTrainer
         trainer = CustomTrainer(
             pooler=self.pooler,
             model=self.backbone,
             dataset_format=self.detect_dataset_format(train_ds),
             train_dataset=train_ds,
             eval_dataset=None,
             loss_kwargs=loss_kwargs,
@@ -1446,14 +1550,16 @@
             ),
             **trainer_kwargs
         )
         if torch.__version__ >= "2" and sys.platform != "win32":
             self.backbone = torch.compile(self.backbone)
 
         trainer.train()
+        if argument_kwargs.get('push_to_hub', False):
+            trainer.push_to_hub()
         self.backbone.save_pretrained(output_dir)
 
     def evaluate(self, data: Dataset, batch_size: int = 32, threshold: Optional[float] = None, device: Any = None):
         self.backbone.eval()
         data_collator = AngleDataCollator(
             self.tokenizer,
             return_tensors="pt",
@@ -1464,66 +1570,66 @@
         # for X, y in data.make_iter(random=False):
         for features in tqdm(chunked_iter(data, batch_size), desc='Evaluate'):
             X = data_collator(features)
             y = X.pop('labels', None)
             y_trues.extend(y[::2, 0].detach().cpu().numpy())
             with torch.no_grad():
                 X.to(device or self.device)
-                x_vecs = self.pooler(X).detach().float().cpu().numpy()
+                x_vecs = self.pooler(X,
+                                     pooling_strategy=self.pooling_strategy).detach().float().cpu().numpy()
             x_vecs = l2_normalize(x_vecs)
             pred = (x_vecs[::2] * x_vecs[1::2]).sum(1)
             y_preds.extend(pred)
 
         y_trues, y_preds = np.array(y_trues), np.array(y_preds)
         corrcoef = compute_corrcoef(y_trues, y_preds)
         if threshold is None:
             _, accuracy = optimal_threshold(y_trues, y_preds)
         else:
             accuracy = np.mean((y_trues > 0.5) == (y_preds > threshold))
         return corrcoef, accuracy
 
-    def set_prompt(self, prompt: str = Prompts.A):
-        self.prompt = prompt
-        if self.prompt is not None:
-            logger.info('Prompt is set, the prompt will be automatically applied during the encoding phase. '
-                        'To disable prompt setting, please configure set_prompt(prompt=None)')
-
     def encode(self,
                inputs: Union[List[str], Tuple[str], List[Dict], str],
                max_length: Optional[int] = None,
                end_with_eos: bool = False,
                to_numpy: bool = True,
                layer_index: int = -1,
+               embedding_start: int = 0,
                embedding_size: Optional[int] = None,
-               device: Optional[Any] = None):
+               device: Optional[Any] = None,
+               prompt: Optional[str] = None):
         """
         encode texts.
 
         :param inputs: Union[List[str], Tuple[str], List[Dict], str]. Input texts. Required.
         :param max_length: Optional[int]. Default None.
         :param to_numpy: bool. Default True.
-        :param layer_index: int. Obtain specific layer's sentence embeddings (for 2DMSE).
-        :param embedding_size: Optional[int]. Specify embedding size (for 2DMSE).
+        :param layer_index: int. Obtain specific layer's sentence embeddings (for Espresso).
+        :param embedding_start: int. Specify the start position of the embedding (for Espresso).
+        :param embedding_size: Optional[int]. Specify embedding size (for Espresso).
+            The embeddings from embedding_start to embedding_start+embedding_size will be returned.
         :param device: Optional[Any]. Default None.
+        :param prompt: Optional[str]. Default None.
         """
         if layer_index != -1 and self.full_backbone is None:
             self.full_backbone = copy.deepcopy(self.backbone)
 
         if layer_index != -1:
             self.backbone.encoder.layer = self.full_backbone.encoder.layer[:layer_index]
 
         if device is None:
             device = self.device
         self.backbone.eval()
         if not isinstance(inputs, (tuple, list)):
             inputs = [inputs]
-        if self.prompt is not None:
+        if prompt is not None:
             for i, obj in enumerate(inputs):
                 assert isinstance(obj, dict), 'The prompt has been set, please pass a dict like {"prompt_key": "text"}'
-                inputs[i] = self.prompt.format(**obj)
+                inputs[i] = prompt.format(**obj)
         max_length = max_length or self.max_length
         if end_with_eos:
             max_length -= 1
 
         if end_with_eos:
             tok = self.tokenizer(
                 inputs,
@@ -1538,14 +1644,24 @@
                 inputs,
                 padding='longest',
                 max_length=max_length or self.max_length,
                 truncation=True,
                 return_tensors='pt')
         tok.to(device)
         with torch.no_grad():
-            output = self.pooler(tok, layer_index=layer_index, embedding_size=embedding_size)
+            output = self.pooler(tok,
+                                 layer_index=layer_index,
+                                 embedding_start=embedding_start,
+                                 embedding_size=embedding_size)
         if to_numpy:
             return output.float().detach().cpu().numpy()
         return output
 
-    def export_onnx(self):
-        pass
+    def push_to_hub(self, hub_model_id: str, private: bool = True, **kwargs):
+        """ push model to hub
+
+        :param hub_model_id: str, hub model id.
+        :param private: bool, whether push to private repo. Default True.
+        :param kwargs: other kwargs for `push_to_hub` method.
+        """
+        self.tokenizer.push_to_hub(hub_model_id, private=private, **kwargs)
+        self.backbone.push_to_hub(hub_model_id, private=private, **kwargs)
```

### Comparing `angle_emb-0.3.9/angle_emb/train_cli.py` & `angle_emb-0.4.0/angle_emb/angle_trainer.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,100 +10,116 @@
 
 from angle_emb import AnglE, AngleDataTokenizer
 from angle_emb.utils import logger
 
 
 parser = argparse.ArgumentParser()
 parser.add_argument('--model_name_or_path', type=str, required=True,
-                    help='Specify model_name_or_path to set transformer backbone, default roberta-large')
+                    help='Specify model name or path to set transformer backbone, required')
 parser.add_argument('--pretrained_model_path', type=str, default=None,
                     help='Specify pretrained model path to load pretrained model, default None')
 parser.add_argument('--pretrained_lora_path', type=str, default=None,
                     help='Specify pretrained lora path to load lora, default None')
 parser.add_argument('--train_name_or_path', type=str, required=True,
                     help='Specify huggingface datasets name or local file path for train set, required')
 parser.add_argument('--train_subset_name', type=str, default=None,
-                    help='Specify huggingface datasets subset name for train set')
+                    help='Specify huggingface datasets subset name for train set, default None')
 parser.add_argument('--train_split_name', type=str, default='train',
-                    help='Specify huggingface datasets split name for train set, Default `train`')
+                    help='Specify huggingface datasets split name for train set, default `train`')
 parser.add_argument('--valid_name_or_path', type=str, default=None,
-                    help='Specify huggingface datasets name or local file path for valid set.')
+                    help='Specify huggingface datasets name or local file path for valid set, default None.')
 parser.add_argument('--valid_subset_name', type=str, default=None,
-                    help='Specify huggingface datasets subset name for valid set')
+                    help='Specify huggingface datasets subset name for valid set, default None')
+parser.add_argument('--valid_split_name', type=str, default='train',
+                    help='Specify huggingface datasets split name for valid set, default `train`')
 parser.add_argument('--prompt_template', type=str, default=None,
-                    help='Specify prompt_template like "Instruct: xxx\nInput: {text}", default None')
+                    help='Specify prompt_template like "xxx: {text}", default None.'
+                         'This prompt will be applied for all text columns.'
+                         'If you want to specify different prompts for different text columns,'
+                         'please handle it in the preprocessing step.')
 parser.add_argument('--save_dir', type=str, default=None,
                     help='Specify save dir, default None')
-parser.add_argument('--seed', type=int, default=42,
-                    help='Specify random seed, default 42')
+parser.add_argument('--seed', type=int, default=-1,
+                    help='Specify random seed, default -1')
 parser.add_argument('--dataset_seed', type=int, default=None,
                     help='Specify dataset random seed, default None')
 parser.add_argument('--workers', type=int, default=2,
                     help='Specify dataset workers, default 2')
-parser.add_argument('--w1', type=float, default=1.0,
-                    help='Specify w1 (cosine), default 1.0')
-parser.add_argument('--w2', type=float, default=1.0,
-                    help='Specify w2 (ibn), default 1.0')
-parser.add_argument('--w3', type=float, default=1.0,
-                    help='Specify w3 (angle), default 1.0')
+parser.add_argument('--cosine_w', type=float, default=1.0,
+                    help='Specify weight for cosine loss, default 1.0')
+parser.add_argument('--ibn_w', type=float, default=1.0,
+                    help='Specify weight for ibn loss, default 1.0')
+parser.add_argument('--angle_w', type=float, default=1.0,
+                    help='Specify weight for angle loss, default 1.0')
 parser.add_argument('--angle_tau', type=float, default=20.0,
                     help='Specify angle_tau, default 20.0')
 parser.add_argument('--cosine_tau', type=float, default=20.0,
                     help='Specify cosine_tau, defaut 20.0')
 parser.add_argument('--ibn_tau', type=float, default=20.0,
                     help='Specify ibn_tau, defaut 20.0')
-parser.add_argument('--is_llm', type=int, default=0, choices=[0, 1],
-                    help='Specify is_llm, choices [0, 1], defaut 0')
 parser.add_argument('--apply_lora', type=int, default=0, choices=[0, 1],
-                    help='Specify apply_lora, choices [0, 1], defaut 0')
+                    help='Specify lora flag, choices [0, 1], default 0')
 parser.add_argument('--load_kbit', type=int, default=None, choices=[4, 8, 16],
                     help='Specify kbit training, choices [4, 8, 16], default None')
 parser.add_argument('--lora_r', type=int, default=32,
                     help='Specify lora_r, defaut 32')
 parser.add_argument('--lora_alpha', type=int, default=32,
                     help='Specify lora_alpha, defaut 32')
 parser.add_argument('--lora_dropout', type=float, default=0.1,
                     help='Specify lora_dropout, defaut 0.1')
+parser.add_argument('--lora_target_modules', type=str, default=None,
+                    help='Specify lora_target_modules. comma serves as the splitter, such as `W,b`. Defaut None')
 parser.add_argument('--learning_rate', type=float, default=1e-5,
                     help='Specify learning_rate, defaut 1e-5')
-parser.add_argument('--start_bilayer_index', type=int, default=None,
-                    help='Specify start_bilayer_index, defaut None')
 parser.add_argument('--warmup_steps', type=int, default=100,
                     help='Specify warmup_steps, defaut 100')
 parser.add_argument('--logging_steps', type=int, default=100,
                     help='Specify logging_steps, defaut 100')
 parser.add_argument('--pooling_strategy', type=str, default='cls',
                     help='Specify pooling_strategy from [`cls`, `last`, `avg`, `cls_avg`, `max`], default `cls`')
-parser.add_argument('--epochs', type=int, default=20, help='Specify epochs, default 20')
+parser.add_argument('--tokenizer_padding_side', type=str, default=None, choices=['left', 'right'],
+                    help='specify tokenizer padding side from [`left`, `right`], default None')
+parser.add_argument('--epochs', type=int, default=10, help='Specify epochs, default 10')
+parser.add_argument('--max_steps', type=int, default=-1,
+                    help='Specify max steps, default -1 (Automatically calculated from epochs)')
 parser.add_argument('--save_steps', type=int, default=100, help='Specify save_steps, default 1000')
 parser.add_argument('--batch_size', type=int, default=32, help='Specify batch size, default 32')
 parser.add_argument('--maxlen', type=int, default=512, help='Specify max length, default 512')
+parser.add_argument('--streaming', action='store_true', default=False,
+                    help='Flag to enable streaming mode, default False')
 parser.add_argument('--gradient_accumulation_steps', type=int, default=1,
                     help='Specify gradient_accumulation_steps, default 1')
-parser.add_argument('--torch_dtype', type=str, default='float32',
-                    help='Specify torch_dtype from `auto`, `float32`, `float16`, default float32')
+parser.add_argument('--torch_dtype', type=str, default=None, choices=['auto', 'float32', 'float16', 'bfloat16'],
+                    help='Specify torch_dtype from [`auto`, `float32`, `float16`, `bfloat16`], default None')
 parser.add_argument('--fp16', type=bool, default=None, choices=[0, 1],
                     help='Specify fp16, choices [0, 1], default None')
 parser.add_argument('--push_to_hub', type=int, default=0, choices=[0, 1], help='Specify push_to_hub, default 0')
+parser.add_argument('--hub_private_repo', type=int, default=1, choices=[0, 1],
+                    help='Specify hub_private_repo, default 1')
 parser.add_argument('--hub_model_id', type=str, default=None,
-                    help='Specify push_to_hub_model_id, default None, format like organization/model_id')
-# configure TDMSE
-parser.add_argument('--apply_tdmse', type=int, default=0, choices=[0, 1],
-                    help='Specify apply_tdmse to support 2DMSE training, default 0')
-parser.add_argument('--apply_tdmse_kl', type=int, default=1, choices=[0, 1],
-                    help='Specify apply_tdmse_kl to support 2DMSE training with KL Divergence, default 1')
-parser.add_argument('--tdmse_kl_temperature', type=float, default=1.0,
-                    help='Specify KL temperature for tdmse, default 1.0')
-parser.add_argument('--tdmse_teacher_lambda', type=float, default=1.0,
-                    help='Specify teacher lambda for tdmse, default 1.0')
-parser.add_argument('--tdmse_student_lambda', type=float, default=1.0,
-                    help='Specify student lambda for tdmse, default 1.0')
+                    help='Specify hub_model_id, default None, format like organization/model_id')
+# configure LLM
+parser.add_argument('--is_llm', type=int, default=0, choices=[0, 1],
+                    help='Specify is_llm, choices [0, 1], defaut 0')
+parser.add_argument('--apply_billm', type=int, default=0, choices=[0, 1],
+                    help='Specify apply_billm, choices [0, 1], defaut 0')
+parser.add_argument('--billm_model_class', type=str, default=None,
+                    help='Specify billm model class name, default None')
+# configure ESE
+parser.add_argument('--apply_ese', type=int, default=0, choices=[0, 1],
+                    help='Specify apply_ese to support Espresso Sentence Embedding training, default 0')
+parser.add_argument('--ese_kl_temperature', type=float, default=1.0,
+                    help='Specify KL temperature for ese, default 1.0')
+parser.add_argument('--ese_compression_size', type=int, default=128,
+                    help='Specify compression size for ese, default 128')
 # configure teacher alignment
-parser.add_argument('--fixed_teacher_name_or_path', type=str, default=None,
+parser.add_argument('--teacher_name_or_path', type=str, default=None,
                     help='Specify model_name_or_path for teacher alignment, default None')
+parser.add_argument('--teacher_pooling_strategy', type=str, default='cls',
+                    help='Specify pooling strategy for teacher from [`cls`, `last`, `avg`, `cls_avg`, `max`], default `cls`')  # NOQA
 # configure wandb
 parser.add_argument('--wandb_project', type=str, default=None, help='Specify WANDB_PROJECT, default None')
 parser.add_argument('--wandb_log_model', type=str, default=None, help='Specify WANDB_LOG_MODEL, default None')
 args = parser.parse_args()
 logger.info(f'Args: {args}')
 
 if args.seed is not None and args.seed > 0:
@@ -121,102 +137,129 @@
 
     wandb.login()
 
 if args.torch_dtype == 'float32':
     args.torch_dtype = torch.float32
 elif args.torch_dtype == 'float16':
     args.torch_dtype = torch.float16
+elif args.torch_dtype == 'bfloat16':
+    args.torch_dtype = torch.bfloat16
+
+apply_bfloat16 = None
+if args.torch_dtype == torch.bfloat16:
+    apply_bfloat16 = True
+
+lora_config = {
+    'r': args.lora_r,
+    'lora_alpha': args.lora_alpha,
+    'lora_dropout': args.lora_dropout,
+}
+if args.lora_target_modules is not None:
+    lora_config['target_modules'] = [v.strip() for v in args.lora_target_modules.split(',') if v.strip()]
 
 
 def main():
     model = AnglE(args.model_name_or_path,
                   max_length=args.maxlen,
                   pretrained_model_path=args.pretrained_model_path,
                   pretrained_lora_path=args.pretrained_lora_path,
                   pooling_strategy=args.pooling_strategy,
                   train_mode=True,
-                  is_llm=args.is_llm,
                   apply_lora=args.apply_lora,
-                  lora_config_kwargs={
-                      'r': args.lora_r,
-                      'lora_alpha': args.lora_alpha,
-                      'lora_dropout': args.lora_dropout,
-                  },
+                  lora_config_kwargs=lora_config,
                   load_kbit=args.load_kbit,
-                  torch_dtype=args.torch_dtype)
-
-    if args.start_bilayer_index is not None:
-        model.backbone.set_start_bilayer_index(args.start_bilayer_index)
+                  torch_dtype=args.torch_dtype,
+                  apply_bfloat16=apply_bfloat16,
+                  tokenizer_padding_side=args.tokenizer_padding_side,
+                  is_llm=args.is_llm,
+                  apply_billm=args.apply_billm,
+                  billm_model_class=args.billm_model_class)
 
     if os.path.exists(args.train_name_or_path):
-        ds = load_dataset('json', data_files=[args.train_name_or_path])
+        ds = load_dataset('json',
+                          data_files=[args.train_name_or_path],
+                          num_proc=args.workers,
+                          streaming=args.streaming)
     else:
-        ds = load_dataset(args.train_name_or_path, args.train_subset_name)
+        ds = load_dataset(args.train_name_or_path,
+                          args.train_subset_name,
+                          num_proc=args.workers,
+                          streaming=args.streaming)
 
     logger.info('Dataset overview:')
     print(ds)
     logger.info('Processing train...')
-    train_ds = ds[args.train_split_name].shuffle(args.dataset_seed).map(
-        AngleDataTokenizer(model.tokenizer, model.max_length,
-                           prompt_template=args.prompt_template), num_proc=args.workers)
+    if args.streaming:
+        train_ds = ds[args.train_split_name].shuffle(args.dataset_seed).map(
+            AngleDataTokenizer(model.tokenizer, model.max_length, prompt_template=args.prompt_template),
+            num_proc=args.workers)
+    else:
+        train_ds = ds[args.train_split_name].shuffle(args.dataset_seed).map(
+            AngleDataTokenizer(model.tokenizer, model.max_length, prompt_template=args.prompt_template),
+            num_proc=args.workers)
 
     valid_ds = None
     if valid_ds is None and args.valid_name_or_path is not None:
         logger.info('Validation detected, processing validation...')
         if os.path.exists(args.valid_name_or_path):
-            valid_ds = load_dataset('json', data_files=[args.valid_name_or_path])
+            valid_ds = load_dataset('json', data_files=[args.valid_name_or_path], num_proc=args.workers)
         else:
-            valid_ds = load_dataset(args.valid_name_or_path, args.valid_subset_name)
-        valid_ds = valid_ds[args.valid_subset_name or 'train'].map(
-            AngleDataTokenizer(model.tokenizer, model.max_length,
-                               prompt_template=args.prompt_template), num_proc=args.workers)
+            if args.valid_subset_name is not None:
+                valid_ds = load_dataset(args.valid_name_or_path, args.valid_subset_name, num_proc=args.workers)
+            else:
+                valid_ds = load_dataset(args.valid_name_or_path, num_proc=args.workers)
+        valid_ds = valid_ds[args.valid_split_name or 'train'].map(
+            AngleDataTokenizer(model.tokenizer, model.max_length, prompt_template=args.prompt_template),
+            num_proc=args.workers)
 
     argument_kwargs = {}
     if args.push_to_hub:
         assert args.hub_model_id is not None, 'Please specify hub_mode_id via --hub_model_id xxx'
-        argument_kwargs['push_to_hub'] = True,
+        argument_kwargs['push_to_hub'] = True
+        argument_kwargs['hub_private_repo'] = bool(args.hub_private_repo)
         argument_kwargs['hub_model_id'] = args.hub_model_id
     if args.wandb_project is not None:
         argument_kwargs['report_to'] = 'wandb'
+    if args.max_steps > 0:
+        argument_kwargs['max_steps'] = args.max_steps
 
     trainer_kwargs = None
-    if args.fixed_teacher_name_or_path is not None:
+    if args.teacher_name_or_path is not None:
         trainer_kwargs = {
-            'fixed_teacher_name_or_path': args.fixed_teacher_name_or_path
+            'teacher_name_or_path': args.teacher_name_or_path,
+            'teacher_pooling_strategy': args.teacher_pooling_strategy,
         }
-    if args.apply_tdmse:
+    if args.apply_ese:
         trainer_kwargs = trainer_kwargs or {}
         trainer_kwargs = dict(trainer_kwargs, **{
-            'apply_tdmse_kl': args.apply_tdmse_kl,
-            'tdmse_kl_temperature': args.tdmse_kl_temperature,
-            'tdmse_teacher_lambda': args.tdmse_teacher_lambda,
-            'tdmse_student_lambda': args.tdmse_student_lambda,
+            'ese_kl_temperature': args.ese_kl_temperature,
+            'ese_compression_size': args.ese_compression_size,
         })
 
     model.fit(
         train_ds=train_ds,
         valid_ds=valid_ds,
         output_dir=args.save_dir,
         batch_size=args.batch_size,
         epochs=args.epochs,
         learning_rate=args.learning_rate,
         save_steps=args.save_steps,
         warmup_steps=args.warmup_steps,
         logging_steps=args.logging_steps,
         gradient_accumulation_steps=args.gradient_accumulation_steps,
         loss_kwargs={
-            'w1': args.w1,
-            'w2': args.w2,
-            'w3': args.w3,
+            'cosine_w': args.cosine_w,
+            'ibn_w': args.ibn_w,
+            'angle_w': args.angle_w,
             'cosine_tau': args.cosine_tau,
             'ibn_tau': args.ibn_tau,
             'angle_tau': args.angle_tau,
         },
         fp16=args.fp16,
         argument_kwargs=argument_kwargs,
-        apply_tdmse=args.apply_tdmse,
+        apply_ese=args.apply_ese,
         trainer_kwargs=trainer_kwargs,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `angle_emb-0.3.9/angle_emb.egg-info/PKG-INFO` & `angle_emb-0.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: angle-emb
-Version: 0.3.9
+Name: angle_emb
+Version: 0.4.0
 Summary: AnglE-optimize Text Embeddings
 Author: sean lee
 Author-email: xmlee97@gmail.com
 Keywords: angle_emb
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -16,253 +16,221 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <small>EN | [简体中文](README_zh.md) </small>
 
-# [AnglE📐: Angle-optimized Text Embeddings](https://arxiv.org/abs/2309.12871)
+# AnglE📐
 
 > It is Angle 📐, not Angel 👼.
 
-🔥 **A New SOTA** for Semantic Textual Similarity! 
-
-
-🔥 **Our universal sentence embedding [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) achieves SOTA on the [MTEB Leaderboard](https://huggingface.co/spaces/mteb/leaderboard) with an average score of 64.64!**
-
+📘 document: https://angle.readthedocs.io/en/latest/index.html
 
 <a href="https://arxiv.org/abs/2309.12871">
-    <img src="https://img.shields.io/badge/Arxiv-2306.06843-yellow.svg?style=flat-square" alt="https://arxiv.org/abs/2309.12871" />
+    <img src="https://img.shields.io/badge/Arxiv-2309.12871-yellow.svg?style=flat-square" alt="https://arxiv.org/abs/2309.12871" />
 </a>
 <a href="https://pypi.org/project/angle_emb/">
     <img src="https://img.shields.io/pypi/v/angle_emb?style=flat-square" alt="PyPI version" />
 </a>
 <a href="https://pypi.org/project/angle_emb/">
     <img src="https://img.shields.io/pypi/dm/angle_emb?style=flat-square" alt="PyPI Downloads" />
 </a>
-<a href="http://makeapullrequest.com">
-    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="http://makeapullrequest.com" />
+<a href="https://angle.readthedocs.io/en/latest/index.html">
+    <img src="https://readthedocs.org/projects/angle/badge/?version=latest&style=flat-square" alt="Read the docs" />
 </a>
 
+
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sick-r-1)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sick-r-1?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts16)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts16?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts15)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts15?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts14)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts14?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts13)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts13?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts12)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts12?p=angle-optimized-text-embeddings)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-similarity-on-sts-benchmark)](https://paperswithcode.com/sota/semantic-textual-similarity-on-sts-benchmark?p=angle-optimized-text-embeddings)
 
+📢 **Train/Infer Powerful Sentence Embeddings with AnglE.**
+This library is from the paper: [AnglE: Angle-optimized Text Embeddings](https://arxiv.org/abs/2309.12871). It allows for training state-of-the-art BERT/LLM-based sentence embeddings with just a few lines of code. AnglE is also a general sentence embedding inference framework, allowing for infering a variety of transformer-based sentence embeddings.
 
-<details>
-<summary>📊 Results on MTEB Leaderboard [click to expand]</summary>
-<p align='center'>
-<img src='assets/UAE-MTEB.png'>
-</p>
-</details>
-
-<details>
-<summary>📊 Results on STS benchmark [click to expand]</summary>
-<p align='center'>
-<img src='assets/angle-results.png'>
-</p>
-</details>
-
-## 🤗 Pretrained Models
-| 🤗 HF | LoRA Weight | Dependent Backbone | LLM | Language | Prompt | Pooling Strategy | Examples |
-|----|------|------|------|------|------|------|------|
-| [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) |  N | N | N | EN | `Prompts.C` for retrieval purposes, `None` for others | cls | [![Seach Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WOYD6f8gb_wpkUm_57K8pEDgjlGJd6oB?usp=drive_link) |
-| [SeanLee97/angle-llama-13b-nli](https://huggingface.co/SeanLee97/angle-llama-13b-nli) | Y |  NousResearch/Llama-2-13b-hf | Y | EN | `Prompts.A` | last token | / | 
-| [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-7b-nli-v2) | Y |  NousResearch/Llama-2-7b-hf | Y | EN | `Prompts.A` | last token | / |
-| [SeanLee97/angle-llama-7b-nli-20231027](https://huggingface.co/SeanLee97/angle-llama-7b-nli-20231027) | Y |  NousResearch/Llama-2-7b-hf | Y | EN | `Prompts.A` | last token | / |
-| [SeanLee97/angle-bert-base-uncased-nli-en-v1](https://huggingface.co/SeanLee97/angle-bert-base-uncased-nli-en-v1) | N |  N | N | EN | N | `cls_avg` | / |
-| [SeanLee97/angle-roberta-wwm-base-zhnli-v1](https://huggingface.co/SeanLee97/angle-roberta-wwm-base-zhnli-v1) | N |  N | N | ZH-CN | N | `cls` | / |
-| [SeanLee97/angle-llama-7b-zhnli-v1](https://huggingface.co/SeanLee97/angle-llama-7b-zhnli-v1) | Y |  NousResearch/Llama-2-7b-hf | Y | ZH-CN | `Prompts.B` | last token | / |
- 
-💡 If the selected model is a LoRA weight, it must specify the corresponding dependent backbone.
-
-For our STS Experiment, please refer to https://github.com/SeanLee97/AnglE/tree/main/examples/NLI
-
-</details>
-
-## Results
-
-### English STS Results
-
-| Model | STS12 | STS13 | STS14 | STS15 | STS16 | STSBenchmark | SICKRelatedness |  Avg. |
-| ------- |-------|-------|-------|-------|-------|--------------|-----------------|-------|
-| [SeanLee97/angle-llama-7b-nli-20231027](https://huggingface.co/SeanLee97/angle-llama-7b-nli-20231027) | 78.68 | 90.58 | 85.49 | 89.56 | 86.91 |    88.92     |      81.18      | 85.90 |
-| [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-7b-nli-v2) | 79.00 | 90.56 | 85.79 | 89.43 | 87.00 |    88.97     |      80.94      | 85.96 |
-| [SeanLee97/angle-llama-13b-nli](https://huggingface.co/SeanLee97/angle-llama-13b-nli)  | 79.33 | 90.65 | 86.89 | 90.45 | 87.32 |    89.69     |      81.32       | **86.52** |
-| [SeanLee97/angle-bert-base-uncased-nli-en-v1](https://huggingface.co/SeanLee97/angle-bert-base-uncased-nli-en-v1) | 75.09 | 85.56 | 80.66 | 86.44 | 82.47 | 85.16 | 81.23 | 82.37 |
-
-
-### Chinese STS Results
-
-| Model | ATEC | BQ	| LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc | Avg. |
-| ------- |-------|-------|-------|-------|-------|--------------|-----------------|-------|
-| ^[shibing624/text2vec-bge-large-chinese](https://huggingface.co/shibing624/text2vec-bge-large-chinese) | 38.41 | 61.34 | 71.72 | 35.15 | 76.44 | 71.81 | 63.15 | 59.72 |
-| ^[shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase) |	44.89 | 63.58 | 74.24 | 40.90 | 78.93 | 76.70 | 63.30 | 63.08 |
-| [SeanLee97/angle-roberta-wwm-base-zhnli-v1](https://huggingface.co/SeanLee97/angle-roberta-wwm-base-zhnli-v1) | 49.49 | 72.47 | 78.33 | 59.13 | 77.14 |    72.36     |      60.53      | **67.06** |
-| [SeanLee97/angle-llama-7b-zhnli-v1](https://huggingface.co/SeanLee97/angle-llama-7b-zhnli-v1) | 50.44 | 71.95 | 78.90 | 56.57 | 81.11 | 68.11 | 52.02 | 65.59 |
+## ✨ Features
 
-^ denotes baselines, their results are retrieved from: https://github.com/shibing624/text2vec
+**Loss**:
+- 📐 AnglE loss
+- ⚖ Contrastive loss
+- 📏 CoSENT loss
+- ☕️ Espresso loss (previously known as 2DMSE, detail: [README_ESE](README_ESE.md))
 
+**Backbones**:
+- BERT-based models (BERT, RoBERTa, ELECTRA, ALBERT, etc.)
+- LLM-based models (LLaMA, Mistral, Qwen, etc.)
+- Bi-directional LLM-based models (LLaMA, Mistral, Qwen, OpenELMo, etc.. refer to: https://github.com/WhereIsAI/BiLLM)
 
-## Usage
+**Training**:
+- Single-GPU training
+- Multi-GPU training
 
-AnglE supports two APIs, one is the `transformers` API, the other is the `AnglE` API. If you want to use the `AnglE` API, please install AnglE first:
 
-```bash
-python -m pip install -U angle-emb
-```
+> <a href="http://makeapullrequest.com"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="http://makeapullrequest.com" /></a> 
+    More features will be added in the future. 
 
-### UAE
+## 🏆 Achievements
 
-1) For Retrieval Purposes
+📅  May 16, 2024 | Paper "[AnglE: Angle-optimized Text Embeddings](https://arxiv.org/abs/2309.12871)" is accepted by ACL 2024 Main Conference.
 
-For retrieval purposes, please use the prompt `Prompts.C`.
+📅  Mar 13, 2024 | Paper "[BeLLM: Backward Dependency Enhanced Large Language Model for Sentence Embeddings](https://arxiv.org/abs/2311.05296)" is accepted by NAACL 2024 Main Conference.
 
-```python
-from angle_emb import AnglE, Prompts
 
-angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1', pooling_strategy='cls').cuda()
-angle.set_prompt(prompt=Prompts.C)
-vec = angle.encode({'text': 'hello world'}, to_numpy=True)
-print(vec)
-vecs = angle.encode([{'text': 'hello world1'}, {'text': 'hello world2'}], to_numpy=True)
-print(vecs)
-```
+📅  Mar 8, 2024 | 🍞 [mixedbread's embedding](https://www.mixedbread.ai/blog/mxbai-embed-large-v1) ([mixedbread-ai/mxbai-embed-large-v1](https://huggingface.co/mixedbread-ai/mxbai-embed-large-v1)) achieves SOTA on the [MTEB Leaderboard](https://huggingface.co/spaces/mteb/leaderboard) with an average score of **64.68**! The model is trained using AnglE. Congrats mixedbread!
 
-2) For non-Retrieval Purposes
 
-```python
-from angle_emb import AnglE
+📅  Dec 4, 2023 | Our universal sentence embedding [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) achieves SOTA on the [MTEB Leaderboard](https://huggingface.co/spaces/mteb/leaderboard) with an average score of **64.64**! The model is trained using AnglE.
+
+
+📅 Dec, 2023 | AnglE achieves SOTA performance on the STS Bechmark Semantic Textual Similarity! 
 
-angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1', pooling_strategy='cls').cuda()
-vec = angle.encode('hello world', to_numpy=True)
-print(vec)
-vecs = angle.encode(['hello world1', 'hello world2'], to_numpy=True)
-print(vecs)
-```
 
-<details>
-<summary>Difference between retrieval and non-retrieval sentence embeddings. [click to expand]</summary>
+## 🤗 Official Pretrained Models
 
-In UAE, we use different approaches for retrieval and non-retrieval tasks, each serving a different purpose. 
+BERT-based models:
 
-**Retrieval tasks aim to find relevant documents, and as a result, the related documents may not have strict semantic similarities to each other.**
+|  🤗 HF | Max Tokens | Pooling Strategy | Scenario |
+|----|------|------|------|
+| [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) | 512 | cls | English, General-purpose |
+| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) |  512 | cls | Code Similarity |
 
-For instance, when querying "How about ChatGPT?", the related documents are those that contain information related to "ChatGPT," such as "ChatGPT is amazing..." or "ChatGPT is bad....".
+LLM-based models:
 
-Conversely, **non-retrieval tasks, such as semantic textual similarity, require sentences that are semantically similar.**
+| 🤗 HF (lora weight) | Backbone | Max Tokens | Prompts |  Pooling Strategy | Scenario  |
+|----|------|------|------|------|------|
+| [SeanLee97/angle-llama-13b-nli](https://huggingface.co/SeanLee97/angle-llama-13b-nli) | NousResearch/Llama-2-13b-hf | 4096 | `Prompts.A` | last token | English, Similarity Measurement | 
+| [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-7b-nli-v2) | NousResearch/Llama-2-7b-hf | 4096 | `Prompts.A` | last token | English, Similarity Measurement | 
 
-For example, a sentence semantically similar to "How about ChatGPT?" could be "What is your opinion about ChatGPT?".
 
-To distinguish between these two types of tasks, we use different prompts. 
+## 🚀 Quick Start
 
-For retrieval tasks, we use the prompt "Represent this sentence for searching relevant passages: {text}" (Prompts.C in angle_emb). 
+### ⬇️ Installation
 
-For non-retrieval tasks, we set the prompt to empty, i.e., just input your text without specifying a prompt.
+```bash
+python -m pip install -U angle-emb
+```
 
-So, if your scenario is retrieval-related, it is highly recommended to set the prompt with angle.set_prompt(prompt=Prompts.C). If not, leave the prompt empty or use angle.set_prompt(prompt=None).
-</details>
+### ⌛ Load BERT-based Model
 
-### Angle-LLaMA
+1) **With Prompts**: You can specify a prompt with `prompt=YOUR_PROMPT` in `encode` method. If set a prompt, the inputs should be a list of dict or a single dict with key `text`, where `text` is the placeholder in the prompt for the input text. You can use other placeholder names. We provide a set of predefined prompts in `Prompts` class, you can check them via `Prompts.list_prompts()`.
 
-1) AnglE
 ```python
 from angle_emb import AnglE, Prompts
+from angle_emb.utils import cosine_similarity
 
-angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf', pretrained_lora_path='SeanLee97/angle-llama-7b-nli-v2')
 
-print('All predefined prompts:', Prompts.list_prompts())
-angle.set_prompt(prompt=Prompts.A)
-print('prompt:', angle.prompt)
-vec = angle.encode({'text': 'hello world'}, to_numpy=True)
-print(vec)
-vecs = angle.encode([{'text': 'hello world1'}, {'text': 'hello world2'}], to_numpy=True)
-print(vecs)
+angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1', pooling_strategy='cls').cuda()
+# For retrieval tasks, we use `Prompts.C` as the prompt for the query when using UAE-Large-V1 (no need to specify prompt for documents).
+# When specify prompt, the inputs should be a list of dict with key 'text'
+qv = angle.encode({'text': 'what is the weather?'}, to_numpy=True, prompt=Prompts.C)
+doc_vecs = angle.encode([
+    'The weather is great!',
+    'it is rainy today.',
+    'i am going to bed'
+], to_numpy=True)
+
+for dv in doc_vecs:
+    print(cosine_similarity(qv[0], dv))
 ```
 
-2) transformers
+2) **Without Prompts**: no need to specify a prompt. Just input a list of strings or a single string.
 
 ```python
-from angle_emb import AnglE, Prompts
-from transformers import AutoModelForCausalLM, AutoTokenizer
-from peft import PeftModel, PeftConfig
+from angle_emb import AnglE
+from angle_emb.utils import cosine_similarity
 
-peft_model_id = 'SeanLee97/angle-llama-7b-nli-v2'
-config = PeftConfig.from_pretrained(peft_model_id)
-tokenizer = AutoTokenizer.from_pretrained(config.base_model_name_or_path)
-model = AutoModelForCausalLM.from_pretrained(config.base_model_name_or_path).bfloat16().cuda()
-model = PeftModel.from_pretrained(model, peft_model_id).cuda()
-
-def decorate_text(text: str):
-    return Prompts.A.format(text=text)
-
-inputs = 'hello world!'
-tok = tokenizer([decorate_text(inputs)], return_tensors='pt')
-for k, v in tok.items():
-    tok[k] = v.cuda()
-vec = model(output_hidden_states=True, **tok).hidden_states[-1][:, -1].float().detach().cpu().numpy()
-print(vec)
+
+angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1', pooling_strategy='cls').cuda()
+# for non-retrieval tasks, we don't need to specify prompt when using UAE-Large-V1.
+doc_vecs = angle.encode([
+    'The weather is great!',
+    'The weather is very good!',
+    'i am going to bed'
+])
+
+for i, dv1 in enumerate(doc_vecs):
+    for dv2 in doc_vecs[i+1:]:
+        print(cosine_similarity(dv1, dv2))
 ```
 
-### Angle-BERT
 
-1) AnglE
+### ⌛ Load LLM-based Models
+
+If the pretrained weight is a LoRA-based model, you need to specify the backbone via `model_name_or_path` and specify the LoRA path via the `pretrained_lora_path` in `from_pretrained` method. 
+
 ```python
-from angle_emb import AnglE
+from angle_emb import AnglE, Prompts
 
-angle = AnglE.from_pretrained('SeanLee97/angle-bert-base-uncased-nli-en-v1', pooling_strategy='cls_avg').cuda()
-vec = angle.encode('hello world', to_numpy=True)
+angle = AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
+                              pretrained_lora_path='SeanLee97/angle-llama-7b-nli-v2',
+                              pooling_strategy='last',
+                              is_llm=True,
+                              torch_dtype='float16')
+
+print('All predefined prompts:', Prompts.list_prompts())
+vec = angle.encode({'text': 'hello world'}, to_numpy=True, prompt=Prompts.A)
 print(vec)
-vecs = angle.encode(['hello world1', 'hello world2'], to_numpy=True)
+vecs = angle.encode([{'text': 'hello world1'}, {'text': 'hello world2'}], to_numpy=True, prompt=Prompts.A)
 print(vecs)
 ```
 
-2) transformers
+### ⌛ Load Third-party Models
+
+You can load any transformer-based third-party models such as `mixedbread-ai/mxbai-embed-large-v1`, `sentence-transformers/all-MiniLM-L6-v2`, and `BAAI/bge-large-en-v1.5` using `angle_emb`.
+
+Here is an example:
 
 ```python
-import torch
-from transformers import AutoModel, AutoTokenizer
+from angle_emb import AnglE
 
-model_id = 'SeanLee97/angle-bert-base-uncased-nli-en-v1'
-tokenizer = AutoTokenizer.from_pretrained(model_id)
-model = AutoModel.from_pretrained(model_id).cuda()
-
-inputs = 'hello world!'
-tok = tokenizer([inputs], return_tensors='pt')
-for k, v in tok.items():
-    tok[k] = v.cuda()
-hidden_state = model(**tok).last_hidden_state
-vec = (hidden_state[:, 0] + torch.mean(hidden_state, dim=1)) / 2.0
+model = AnglE.from_pretrained('mixedbread-ai/mxbai-embed-large-v1', pooling_strategy='cls').cuda()
+vec = model.encode('hello world', to_numpy=True)
 print(vec)
 ```
 
-## Custom Train
 
-### 1. Data Prepation
+## 🕸️ Custom Train
+
+### 🗂️ 1. Data Prepation
 
-We support two dataset formats:
+We currently support three dataset formats:
 
 1) `DatasetFormats.A`: it is a pair format with three columns: `text1`, `text2`, and `label` (0/1).
 
 2) `DatasetFormats.B`: it is a triple format with three columns: `text`, `positive`, and `negative`. `positive` and `negative` store the positive and negative samples of `text`.
 
 3) `DatasetFormats.C`: it is a pair format with two columns: `text`, `positive`. `positive` store the positive sample of `text`.
 
 You need to prepare your data into huggingface `datasets.Dataset` in one of the formats in terms of your supervised data.
 
-### 2. Train
+### 🚂 2. Train with CLI
+
+Use `angle-trainer` to train your AnglE model in cli mode. 
+
+1) Single gpu training:
 
-Use `angle-trainer` to train your AnglE model in cli mode. Usage: `CUDA_VISIBLE_DEVICES=0 angle-trainer --help`
+Usage: 
 
+```bash
+CUDA_VISIBLE_DEVICES=0 angle-trainer --help
+```
 
-### 3. Example
+2) Multi-gpu training:
+
+Usage:
+
+```bash
+CUDA_VISIBLE_DEVICES=0,1 torchrun --nproc_per_node=2 --master_port=1234 -m angle_emb.angle_trainer --help
+```
+
+### 🚂 3. Custom Train
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1h28jHvv_x-0fZ0tItIMjf8rJGp3GcO5V?usp=sharing)
 
 
 ```python
 from datasets import load_dataset
 from angle_emb import AnglE, AngleDataTokenizer
@@ -291,45 +259,73 @@
     epochs=5,
     learning_rate=2e-5,
     save_steps=100,
     eval_steps=1000,
     warmup_steps=0,
     gradient_accumulation_steps=1,
     loss_kwargs={
-        'w1': 1.0,
-        'w2': 1.0,
-        'w3': 1.0,
+        'cosine_w': 1.0,
+        'ibn_w': 1.0,
+        'angle_w': 1.0,
         'cosine_tau': 20,
         'ibn_tau': 20,
-        'angle_tau': 1.0
+        'angle_tau': 20
     },
     fp16=True,
     logging_steps=100
 )
 
 # 5. evaluate
 corrcoef, accuracy = angle.evaluate(test_ds, device=angle.device)
 print('corrcoef:', corrcoef)
 ```
 
-# Citation
+### 💡 Others
+
+- To enable `llm` training, please specify `--is_llm 1` and configure appropriate LoRA hyperparameters.
+- To enable `billm` training, please specify `--apply_billm 1` and configure appropriate `billm_model_class` such as `LLamaForCausalLM` (refer to: https://github.com/WhereIsAI/BiLLM?tab=readme-ov-file#usage).
+- To enable espresso sentence embeddings (ESE), please specify `--apply_ese 1` and configure appropriate ESE hyperparameters via `--ese_kl_temperature float` and `--ese_compression_size integer`.
+- To convert the trained AnglE models to `sentence-transformers`, please run `python scripts/convert_to_sentence_transformers.py --help` for more details.
+
+
+## 💡 4. Fine-tuning Tips
+
+1️⃣ If your dataset format is `DatasetFormats.A`, it is recommended to slightly increase the weight for `cosine_w` or slightly decrease the weight for `ibn_w`.
+
+2️⃣ If your dataset format is `DatasetFormats.B`, it is recommended to set `cosine_w` to 0, and increase the weight for `ibn_w` such as 10 and 20. The `angle_tau` is recommended to set to 20.0.
+
+3️⃣ If your dataset format is `DatasetFormats.C`, only `ibn_w` and `ibn_tau` are effective. You don't need to tune other parameters.
+
+4️⃣ To alleviate information forgetting in fine-tuning, it is better to specify the `teacher_name_or_path`. If the `teacher_name_or_path` equals `model_name_or_path`, it will conduct self-distillation. **It is worth to note that** `teacher_name_or_path` has to have the same tokenizer as `model_name_or_path`. Or it will lead to unexpected results.
+
+
+# 🫡 Citation
 
 You are welcome to use our code and pre-trained models. If you use our code and pre-trained models, please support us by citing our work as follows:
 
 ```bibtex
 @article{li2023angle,
   title={AnglE-optimized Text Embeddings},
   author={Li, Xianming and Li, Jing},
   journal={arXiv preprint arXiv:2309.12871},
   year={2023}
 }
 ```
 
-# ChangeLogs
+# 📜 ChangeLogs
 
 | 📅 | Description |
 |----|------|
+| 2024 May 21 |  support Espresso Sentence Embeddings  |
 | 2024 Feb 7 |  support training with only positive pairs (`DatasetFormats.C`)  |
-| 2024 Jan 11 |  refactor to support `angle-trainer` and BeLLM  |
 | 2023 Dec 4 |  Release a universal English sentence embedding model: [WhereIsAI/UAE-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1)  |
 | 2023 Nov 2 |  Release an English pretrained model: `SeanLee97/angle-llama-13b-nli` |
 | 2023 Oct 28 |  Release two chinese pretrained models: `SeanLee97/angle-roberta-wwm-base-zhnli-v1` and `SeanLee97/angle-llama-7b-zhnli-v1`; Add chinese README.md |
+
+# 📧 Contact
+
+If you have any questions or suggestions, please feel free to contact us via email: xmlee97@gmail.com
+
+# © License
+
+This project is licensed under the MIT License.
+For the pretrained models, please refer to the corresponding license of the models.
```

#### html2text {}

```diff
@@ -1,24 +1,20 @@
-Metadata-Version: 2.1 Name: angle-emb Version: 0.3.9 Summary: AnglE-optimize
+Metadata-Version: 2.1 Name: angle_emb Version: 0.4.0 Summary: AnglE-optimize
 Text Embeddings Author: sean lee Author-email: xmlee97@gmail.com Keywords:
 angle_emb Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Description-Content-Type:
 text/markdown License-File: LICENSE EN | [ç®ä½ä¸­æ](README_zh.md) #
-[AnglEð: Angle-optimized Text Embeddings](https://arxiv.org/abs/2309.12871)
-> It is Angle ð, not Angel ð¼. ð¥ **A New SOTA** for Semantic Textual
-Similarity! ð¥ **Our universal sentence embedding [WhereIsAI/UAE-Large-V1]
-(https://huggingface.co/WhereIsAI/UAE-Large-V1) achieves SOTA on the [MTEB
-Leaderboard](https://huggingface.co/spaces/mteb/leaderboard) with an average
-score of 64.64!** _[_h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_3_0_9_._1_2_8_7_1_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I
-_D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_:_/_/_m_a_k_e_a_p_u_l_l_r_e_q_u_e_s_t_._c_o_m_][![PWC](https://img.shields.io/
+AnglEð > It is Angle ð, not Angel ð¼. ð document: https://
+angle.readthedocs.io/en/latest/index.html _[_h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_3_0_9_._1_2_8_7_1_]
+_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _D_o_w_n_l_o_a_d_s_]_[_R_e_a_d_ _t_h_e_ _d_o_c_s_][![PWC](https://img.shields.io/
 endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-
 embeddings/semantic-textual-similarity-on-sick-r-1)](https://
 paperswithcode.com/sota/semantic-textual-similarity-on-sick-r-1?p=angle-
 optimized-text-embeddings) [![PWC](https://img.shields.io/
 endpoint.svg?url=https://paperswithcode.com/badge/angle-optimized-text-
 embeddings/semantic-textual-similarity-on-sts16)](https://paperswithcode.com/
 sota/semantic-textual-similarity-on-sts16?p=angle-optimized-text-embeddings) [!
@@ -35,157 +31,155 @@
 text-embeddings) [![PWC](https://img.shields.io/endpoint.svg?url=https://
 paperswithcode.com/badge/angle-optimized-text-embeddings/semantic-textual-
 similarity-on-sts12)](https://paperswithcode.com/sota/semantic-textual-
 similarity-on-sts12?p=angle-optimized-text-embeddings) [![PWC](https://
 img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/angle-
 optimized-text-embeddings/semantic-textual-similarity-on-sts-benchmark)](https:
 //paperswithcode.com/sota/semantic-textual-similarity-on-sts-benchmark?p=angle-
-optimized-text-embeddings) ð Results on MTEB Leaderboard [click to expand]
-                             [assets/UAE-MTEB.png]
-ð Results on STS benchmark [click to expand]
-                          [assets/angle-results.png]
-## ð¤ Pretrained Models | ð¤ HF | LoRA Weight | Dependent Backbone | LLM |
-Language | Prompt | Pooling Strategy | Examples | |----|------|------|------|--
-----|------|------|------| | [WhereIsAI/UAE-Large-V1](https://huggingface.co/
-WhereIsAI/UAE-Large-V1) | N | N | N | EN | `Prompts.C` for retrieval purposes,
-`None` for others | cls | [![Seach Demo](https://colab.research.google.com/
-assets/colab-badge.svg)](https://colab.research.google.com/drive/
-1WOYD6f8gb_wpkUm_57K8pEDgjlGJd6oB?usp=drive_link) | | [SeanLee97/angle-llama-
-13b-nli](https://huggingface.co/SeanLee97/angle-llama-13b-nli) | Y |
-NousResearch/Llama-2-13b-hf | Y | EN | `Prompts.A` | last token | / | |
+optimized-text-embeddings) ð¢ **Train/Infer Powerful Sentence Embeddings with
+AnglE.** This library is from the paper: [AnglE: Angle-optimized Text
+Embeddings](https://arxiv.org/abs/2309.12871). It allows for training state-of-
+the-art BERT/LLM-based sentence embeddings with just a few lines of code. AnglE
+is also a general sentence embedding inference framework, allowing for infering
+a variety of transformer-based sentence embeddings. ## â¨ Features **Loss**: -
+ð AnglE loss - â Contrastive loss - ð CoSENT loss - âï¸ Espresso
+loss (previously known as 2DMSE, detail: [README_ESE](README_ESE.md))
+**Backbones**: - BERT-based models (BERT, RoBERTa, ELECTRA, ALBERT, etc.) -
+LLM-based models (LLaMA, Mistral, Qwen, etc.) - Bi-directional LLM-based models
+(LLaMA, Mistral, Qwen, OpenELMo, etc.. refer to: https://github.com/WhereIsAI/
+BiLLM) **Training**: - Single-GPU training - Multi-GPU training > _[_h_t_t_p_:_/_/
+_m_a_k_e_a_p_u_l_l_r_e_q_u_e_s_t_._c_o_m_]More features will be added in the future. ## ð
+Achievements ð May 16, 2024 | Paper "[AnglE: Angle-optimized Text
+Embeddings](https://arxiv.org/abs/2309.12871)" is accepted by ACL 2024 Main
+Conference. ð Mar 13, 2024 | Paper "[BeLLM: Backward Dependency Enhanced
+Large Language Model for Sentence Embeddings](https://arxiv.org/abs/
+2311.05296)" is accepted by NAACL 2024 Main Conference. ð Mar 8, 2024 | ð
+[mixedbread's embedding](https://www.mixedbread.ai/blog/mxbai-embed-large-v1) (
+[mixedbread-ai/mxbai-embed-large-v1](https://huggingface.co/mixedbread-ai/
+mxbai-embed-large-v1)) achieves SOTA on the [MTEB Leaderboard](https://
+huggingface.co/spaces/mteb/leaderboard) with an average score of **64.68**! The
+model is trained using AnglE. Congrats mixedbread! ð Dec 4, 2023 | Our
+universal sentence embedding [WhereIsAI/UAE-Large-V1](https://huggingface.co/
+WhereIsAI/UAE-Large-V1) achieves SOTA on the [MTEB Leaderboard](https://
+huggingface.co/spaces/mteb/leaderboard) with an average score of **64.64**! The
+model is trained using AnglE. ð Dec, 2023 | AnglE achieves SOTA performance
+on the STS Bechmark Semantic Textual Similarity! ## ð¤ Official Pretrained
+Models BERT-based models: | ð¤ HF | Max Tokens | Pooling Strategy | Scenario
+| |----|------|------|------| | [WhereIsAI/UAE-Large-V1](https://
+huggingface.co/WhereIsAI/UAE-Large-V1) | 512 | cls | English, General-purpose |
+| [WhereIsAI/UAE-Code-Large-V1](https://huggingface.co/WhereIsAI/UAE-Large-V1)
+| 512 | cls | Code Similarity | LLM-based models: | ð¤ HF (lora weight) |
+Backbone | Max Tokens | Prompts | Pooling Strategy | Scenario | |----|------|--
+----|------|------|------| | [SeanLee97/angle-llama-13b-nli](https://
+huggingface.co/SeanLee97/angle-llama-13b-nli) | NousResearch/Llama-2-13b-hf |
+4096 | `Prompts.A` | last token | English, Similarity Measurement | |
 [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/angle-llama-
-7b-nli-v2) | Y | NousResearch/Llama-2-7b-hf | Y | EN | `Prompts.A` | last token
-| / | | [SeanLee97/angle-llama-7b-nli-20231027](https://huggingface.co/
-SeanLee97/angle-llama-7b-nli-20231027) | Y | NousResearch/Llama-2-7b-hf | Y |
-EN | `Prompts.A` | last token | / | | [SeanLee97/angle-bert-base-uncased-nli-
-en-v1](https://huggingface.co/SeanLee97/angle-bert-base-uncased-nli-en-v1) | N
-| N | N | EN | N | `cls_avg` | / | | [SeanLee97/angle-roberta-wwm-base-zhnli-
-v1](https://huggingface.co/SeanLee97/angle-roberta-wwm-base-zhnli-v1) | N | N |
-N | ZH-CN | N | `cls` | / | | [SeanLee97/angle-llama-7b-zhnli-v1](https://
-huggingface.co/SeanLee97/angle-llama-7b-zhnli-v1) | Y | NousResearch/Llama-2-
-7b-hf | Y | ZH-CN | `Prompts.B` | last token | / | ð¡ If the selected model
-is a LoRA weight, it must specify the corresponding dependent backbone. For our
-STS Experiment, please refer to https://github.com/SeanLee97/AnglE/tree/main/
-examples/NLI ## Results ### English STS Results | Model | STS12 | STS13 | STS14
-| STS15 | STS16 | STSBenchmark | SICKRelatedness | Avg. | | ------- |-------|--
------|-------|-------|-------|--------------|-----------------|-------| |
-[SeanLee97/angle-llama-7b-nli-20231027](https://huggingface.co/SeanLee97/angle-
-llama-7b-nli-20231027) | 78.68 | 90.58 | 85.49 | 89.56 | 86.91 | 88.92 | 81.18
-| 85.90 | | [SeanLee97/angle-llama-7b-nli-v2](https://huggingface.co/SeanLee97/
-angle-llama-7b-nli-v2) | 79.00 | 90.56 | 85.79 | 89.43 | 87.00 | 88.97 | 80.94
-| 85.96 | | [SeanLee97/angle-llama-13b-nli](https://huggingface.co/SeanLee97/
-angle-llama-13b-nli) | 79.33 | 90.65 | 86.89 | 90.45 | 87.32 | 89.69 | 81.32 |
-**86.52** | | [SeanLee97/angle-bert-base-uncased-nli-en-v1](https://
-huggingface.co/SeanLee97/angle-bert-base-uncased-nli-en-v1) | 75.09 | 85.56 |
-80.66 | 86.44 | 82.47 | 85.16 | 81.23 | 82.37 | ### Chinese STS Results | Model
-| ATEC | BQ | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc | Avg. | | ------- |---
-----|-------|-------|-------|-------|--------------|-----------------|-------
-| | ^[shibing624/text2vec-bge-large-chinese](https://huggingface.co/shibing624/
-text2vec-bge-large-chinese) | 38.41 | 61.34 | 71.72 | 35.15 | 76.44 | 71.81 |
-63.15 | 59.72 | | ^[shibing624/text2vec-base-chinese-paraphrase](https://
-huggingface.co/shibing624/text2vec-base-chinese-paraphrase) | 44.89 | 63.58 |
-74.24 | 40.90 | 78.93 | 76.70 | 63.30 | 63.08 | | [SeanLee97/angle-roberta-wwm-
-base-zhnli-v1](https://huggingface.co/SeanLee97/angle-roberta-wwm-base-zhnli-
-v1) | 49.49 | 72.47 | 78.33 | 59.13 | 77.14 | 72.36 | 60.53 | **67.06** | |
-[SeanLee97/angle-llama-7b-zhnli-v1](https://huggingface.co/SeanLee97/angle-
-llama-7b-zhnli-v1) | 50.44 | 71.95 | 78.90 | 56.57 | 81.11 | 68.11 | 52.02 |
-65.59 | ^ denotes baselines, their results are retrieved from: https://
-github.com/shibing624/text2vec ## Usage AnglE supports two APIs, one is the
-`transformers` API, the other is the `AnglE` API. If you want to use the
-`AnglE` API, please install AnglE first: ```bash python -m pip install -
-U angle-emb ``` ### UAE 1) For Retrieval Purposes For retrieval purposes,
-please use the prompt `Prompts.C`. ```python from angle_emb import AnglE,
-Prompts angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1',
-pooling_strategy='cls').cuda() angle.set_prompt(prompt=Prompts.C) vec =
-angle.encode({'text': 'hello world'}, to_numpy=True) print(vec) vecs =
-angle.encode([{'text': 'hello world1'}, {'text': 'hello world2'}],
-to_numpy=True) print(vecs) ``` 2) For non-Retrieval Purposes ```python from
-angle_emb import AnglE angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-V1',
-pooling_strategy='cls').cuda() vec = angle.encode('hello world', to_numpy=True)
-print(vec) vecs = angle.encode(['hello world1', 'hello world2'], to_numpy=True)
-print(vecs) ``` Difference between retrieval and non-retrieval sentence
-embeddings. [click to expand] In UAE, we use different approaches for retrieval
-and non-retrieval tasks, each serving a different purpose. **Retrieval tasks
-aim to find relevant documents, and as a result, the related documents may not
-have strict semantic similarities to each other.** For instance, when querying
-"How about ChatGPT?", the related documents are those that contain information
-related to "ChatGPT," such as "ChatGPT is amazing..." or "ChatGPT is bad....".
-Conversely, **non-retrieval tasks, such as semantic textual similarity, require
-sentences that are semantically similar.** For example, a sentence semantically
-similar to "How about ChatGPT?" could be "What is your opinion about ChatGPT?".
-To distinguish between these two types of tasks, we use different prompts. For
-retrieval tasks, we use the prompt "Represent this sentence for searching
-relevant passages: {text}" (Prompts.C in angle_emb). For non-retrieval tasks,
-we set the prompt to empty, i.e., just input your text without specifying a
-prompt. So, if your scenario is retrieval-related, it is highly recommended to
-set the prompt with angle.set_prompt(prompt=Prompts.C). If not, leave the
-prompt empty or use angle.set_prompt(prompt=None). ### Angle-LLaMA 1) AnglE
-```python from angle_emb import AnglE, Prompts angle = AnglE.from_pretrained
-('NousResearch/Llama-2-7b-hf', pretrained_lora_path='SeanLee97/angle-llama-7b-
-nli-v2') print('All predefined prompts:', Prompts.list_prompts())
-angle.set_prompt(prompt=Prompts.A) print('prompt:', angle.prompt) vec =
-angle.encode({'text': 'hello world'}, to_numpy=True) print(vec) vecs =
-angle.encode([{'text': 'hello world1'}, {'text': 'hello world2'}],
-to_numpy=True) print(vecs) ``` 2) transformers ```python from angle_emb import
-AnglE, Prompts from transformers import AutoModelForCausalLM, AutoTokenizer
-from peft import PeftModel, PeftConfig peft_model_id = 'SeanLee97/angle-llama-
-7b-nli-v2' config = PeftConfig.from_pretrained(peft_model_id) tokenizer =
-AutoTokenizer.from_pretrained(config.base_model_name_or_path) model =
-AutoModelForCausalLM.from_pretrained(config.base_model_name_or_path).bfloat16
-().cuda() model = PeftModel.from_pretrained(model, peft_model_id).cuda() def
-decorate_text(text: str): return Prompts.A.format(text=text) inputs = 'hello
-world!' tok = tokenizer([decorate_text(inputs)], return_tensors='pt') for k, v
-in tok.items(): tok[k] = v.cuda() vec = model(output_hidden_states=True,
-**tok).hidden_states[-1][:, -1].float().detach().cpu().numpy() print(vec) ```
-### Angle-BERT 1) AnglE ```python from angle_emb import AnglE angle =
-AnglE.from_pretrained('SeanLee97/angle-bert-base-uncased-nli-en-v1',
-pooling_strategy='cls_avg').cuda() vec = angle.encode('hello world',
-to_numpy=True) print(vec) vecs = angle.encode(['hello world1', 'hello world2'],
-to_numpy=True) print(vecs) ``` 2) transformers ```python import torch from
-transformers import AutoModel, AutoTokenizer model_id = 'SeanLee97/angle-bert-
-base-uncased-nli-en-v1' tokenizer = AutoTokenizer.from_pretrained(model_id)
-model = AutoModel.from_pretrained(model_id).cuda() inputs = 'hello world!' tok
-= tokenizer([inputs], return_tensors='pt') for k, v in tok.items(): tok[k] =
-v.cuda() hidden_state = model(**tok).last_hidden_state vec = (hidden_state[:,
-0] + torch.mean(hidden_state, dim=1)) / 2.0 print(vec) ``` ## Custom Train ###
-1. Data Prepation We support two dataset formats: 1) `DatasetFormats.A`: it is
-a pair format with three columns: `text1`, `text2`, and `label` (0/1). 2)
+7b-nli-v2) | NousResearch/Llama-2-7b-hf | 4096 | `Prompts.A` | last token |
+English, Similarity Measurement | ## ð Quick Start ### â¬ï¸ Installation
+```bash python -m pip install -U angle-emb ``` ### â Load BERT-based Model 1)
+**With Prompts**: You can specify a prompt with `prompt=YOUR_PROMPT` in
+`encode` method. If set a prompt, the inputs should be a list of dict or a
+single dict with key `text`, where `text` is the placeholder in the prompt for
+the input text. You can use other placeholder names. We provide a set of
+predefined prompts in `Prompts` class, you can check them via
+`Prompts.list_prompts()`. ```python from angle_emb import AnglE, Prompts from
+angle_emb.utils import cosine_similarity angle = AnglE.from_pretrained
+('WhereIsAI/UAE-Large-V1', pooling_strategy='cls').cuda() # For retrieval
+tasks, we use `Prompts.C` as the prompt for the query when using UAE-Large-V1
+(no need to specify prompt for documents). # When specify prompt, the inputs
+should be a list of dict with key 'text' qv = angle.encode({'text': 'what is
+the weather?'}, to_numpy=True, prompt=Prompts.C) doc_vecs = angle.encode([ 'The
+weather is great!', 'it is rainy today.', 'i am going to bed' ], to_numpy=True)
+for dv in doc_vecs: print(cosine_similarity(qv[0], dv)) ``` 2) **Without
+Prompts**: no need to specify a prompt. Just input a list of strings or a
+single string. ```python from angle_emb import AnglE from angle_emb.utils
+import cosine_similarity angle = AnglE.from_pretrained('WhereIsAI/UAE-Large-
+V1', pooling_strategy='cls').cuda() # for non-retrieval tasks, we don't need to
+specify prompt when using UAE-Large-V1. doc_vecs = angle.encode([ 'The weather
+is great!', 'The weather is very good!', 'i am going to bed' ]) for i, dv1 in
+enumerate(doc_vecs): for dv2 in doc_vecs[i+1:]: print(cosine_similarity(dv1,
+dv2)) ``` ### â Load LLM-based Models If the pretrained weight is a LoRA-
+based model, you need to specify the backbone via `model_name_or_path` and
+specify the LoRA path via the `pretrained_lora_path` in `from_pretrained`
+method. ```python from angle_emb import AnglE, Prompts angle =
+AnglE.from_pretrained('NousResearch/Llama-2-7b-hf',
+pretrained_lora_path='SeanLee97/angle-llama-7b-nli-v2',
+pooling_strategy='last', is_llm=True, torch_dtype='float16') print('All
+predefined prompts:', Prompts.list_prompts()) vec = angle.encode({'text':
+'hello world'}, to_numpy=True, prompt=Prompts.A) print(vec) vecs = angle.encode
+([{'text': 'hello world1'}, {'text': 'hello world2'}], to_numpy=True,
+prompt=Prompts.A) print(vecs) ``` ### â Load Third-party Models You can load
+any transformer-based third-party models such as `mixedbread-ai/mxbai-embed-
+large-v1`, `sentence-transformers/all-MiniLM-L6-v2`, and `BAAI/bge-large-en-
+v1.5` using `angle_emb`. Here is an example: ```python from angle_emb import
+AnglE model = AnglE.from_pretrained('mixedbread-ai/mxbai-embed-large-v1',
+pooling_strategy='cls').cuda() vec = model.encode('hello world', to_numpy=True)
+print(vec) ``` ## ð¸ï¸ Custom Train ### ðï¸ 1. Data Prepation We
+currently support three dataset formats: 1) `DatasetFormats.A`: it is a pair
+format with three columns: `text1`, `text2`, and `label` (0/1). 2)
 `DatasetFormats.B`: it is a triple format with three columns: `text`,
 `positive`, and `negative`. `positive` and `negative` store the positive and
 negative samples of `text`. 3) `DatasetFormats.C`: it is a pair format with two
 columns: `text`, `positive`. `positive` store the positive sample of `text`.
 You need to prepare your data into huggingface `datasets.Dataset` in one of the
-formats in terms of your supervised data. ### 2. Train Use `angle-trainer` to
-train your AnglE model in cli mode. Usage: `CUDA_VISIBLE_DEVICES=0 angle-
-trainer --help` ### 3. Example [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/1h28jHvv_x-0fZ0tItIMjf8rJGp3GcO5V?usp=sharing)
-```python from datasets import load_dataset from angle_emb import AnglE,
-AngleDataTokenizer # 1. load pretrained model angle = AnglE.from_pretrained
-('SeanLee97/angle-bert-base-uncased-nli-en-v1', max_length=128,
-pooling_strategy='cls').cuda() # 2. load dataset # `text1`, `text2`, and
-`label` are three required columns. ds = load_dataset('mteb/stsbenchmark-sts')
-ds = ds.map(lambda obj: {"text1": str(obj["sentence1"]), "text2": str(obj
-['sentence2']), "label": obj['score']}) ds = ds.select_columns(["text1",
-"text2", "label"]) # 3. transform data train_ds = ds['train'].shuffle().map
-(AngleDataTokenizer(angle.tokenizer, angle.max_length), num_proc=8) valid_ds =
-ds['validation'].map(AngleDataTokenizer(angle.tokenizer, angle.max_length),
-num_proc=8) test_ds = ds['test'].map(AngleDataTokenizer(angle.tokenizer,
-angle.max_length), num_proc=8) # 4. fit angle.fit( train_ds=train_ds,
-valid_ds=valid_ds, output_dir='ckpts/sts-b', batch_size=32, epochs=5,
-learning_rate=2e-5, save_steps=100, eval_steps=1000, warmup_steps=0,
-gradient_accumulation_steps=1, loss_kwargs={ 'w1': 1.0, 'w2': 1.0, 'w3': 1.0,
-'cosine_tau': 20, 'ibn_tau': 20, 'angle_tau': 1.0 }, fp16=True,
-logging_steps=100 ) # 5. evaluate corrcoef, accuracy = angle.evaluate(test_ds,
-device=angle.device) print('corrcoef:', corrcoef) ``` # Citation You are
-welcome to use our code and pre-trained models. If you use our code and pre-
-trained models, please support us by citing our work as follows: ```bibtex
-@article{li2023angle, title={AnglE-optimized Text Embeddings}, author={Li,
-Xianming and Li, Jing}, journal={arXiv preprint arXiv:2309.12871}, year={2023}
-} ``` # ChangeLogs | ð | Description | |----|------| | 2024 Feb 7 | support
-training with only positive pairs (`DatasetFormats.C`) | | 2024 Jan 11 |
-refactor to support `angle-trainer` and BeLLM | | 2023 Dec 4 | Release a
-universal English sentence embedding model: [WhereIsAI/UAE-Large-V1](https://
-huggingface.co/WhereIsAI/UAE-Large-V1) | | 2023 Nov 2 | Release an English
-pretrained model: `SeanLee97/angle-llama-13b-nli` | | 2023 Oct 28 | Release two
-chinese pretrained models: `SeanLee97/angle-roberta-wwm-base-zhnli-v1` and
-`SeanLee97/angle-llama-7b-zhnli-v1`; Add chinese README.md |
+formats in terms of your supervised data. ### ð 2. Train with CLI Use
+`angle-trainer` to train your AnglE model in cli mode. 1) Single gpu training:
+Usage: ```bash CUDA_VISIBLE_DEVICES=0 angle-trainer --help ``` 2) Multi-gpu
+training: Usage: ```bash CUDA_VISIBLE_DEVICES=0,1 torchrun --nproc_per_node=2 -
+-master_port=1234 -m angle_emb.angle_trainer --help ``` ### ð 3. Custom
+Train [![Open In Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/drive/1h28jHvv_x-
+0fZ0tItIMjf8rJGp3GcO5V?usp=sharing) ```python from datasets import load_dataset
+from angle_emb import AnglE, AngleDataTokenizer # 1. load pretrained model
+angle = AnglE.from_pretrained('SeanLee97/angle-bert-base-uncased-nli-en-v1',
+max_length=128, pooling_strategy='cls').cuda() # 2. load dataset # `text1`,
+`text2`, and `label` are three required columns. ds = load_dataset('mteb/
+stsbenchmark-sts') ds = ds.map(lambda obj: {"text1": str(obj["sentence1"]),
+"text2": str(obj['sentence2']), "label": obj['score']}) ds = ds.select_columns(
+["text1", "text2", "label"]) # 3. transform data train_ds = ds['train'].shuffle
+().map(AngleDataTokenizer(angle.tokenizer, angle.max_length), num_proc=8)
+valid_ds = ds['validation'].map(AngleDataTokenizer(angle.tokenizer,
+angle.max_length), num_proc=8) test_ds = ds['test'].map(AngleDataTokenizer
+(angle.tokenizer, angle.max_length), num_proc=8) # 4. fit angle.fit
+( train_ds=train_ds, valid_ds=valid_ds, output_dir='ckpts/sts-b',
+batch_size=32, epochs=5, learning_rate=2e-5, save_steps=100, eval_steps=1000,
+warmup_steps=0, gradient_accumulation_steps=1, loss_kwargs={ 'cosine_w': 1.0,
+'ibn_w': 1.0, 'angle_w': 1.0, 'cosine_tau': 20, 'ibn_tau': 20, 'angle_tau': 20
+}, fp16=True, logging_steps=100 ) # 5. evaluate corrcoef, accuracy =
+angle.evaluate(test_ds, device=angle.device) print('corrcoef:', corrcoef) ```
+### ð¡ Others - To enable `llm` training, please specify `--is_llm 1` and
+configure appropriate LoRA hyperparameters. - To enable `billm` training,
+please specify `--apply_billm 1` and configure appropriate `billm_model_class`
+such as `LLamaForCausalLM` (refer to: https://github.com/WhereIsAI/
+BiLLM?tab=readme-ov-file#usage). - To enable espresso sentence embeddings
+(ESE), please specify `--apply_ese 1` and configure appropriate ESE
+hyperparameters via `--ese_kl_temperature float` and `--ese_compression_size
+integer`. - To convert the trained AnglE models to `sentence-transformers`,
+please run `python scripts/convert_to_sentence_transformers.py --help` for more
+details. ## ð¡ 4. Fine-tuning Tips 1ï¸â£ If your dataset format is
+`DatasetFormats.A`, it is recommended to slightly increase the weight for
+`cosine_w` or slightly decrease the weight for `ibn_w`. 2ï¸â£ If your dataset
+format is `DatasetFormats.B`, it is recommended to set `cosine_w` to 0, and
+increase the weight for `ibn_w` such as 10 and 20. The `angle_tau` is
+recommended to set to 20.0. 3ï¸â£ If your dataset format is
+`DatasetFormats.C`, only `ibn_w` and `ibn_tau` are effective. You don't need to
+tune other parameters. 4ï¸â£ To alleviate information forgetting in fine-
+tuning, it is better to specify the `teacher_name_or_path`. If the
+`teacher_name_or_path` equals `model_name_or_path`, it will conduct self-
+distillation. **It is worth to note that** `teacher_name_or_path` has to have
+the same tokenizer as `model_name_or_path`. Or it will lead to unexpected
+results. # ð«¡ Citation You are welcome to use our code and pre-trained
+models. If you use our code and pre-trained models, please support us by citing
+our work as follows: ```bibtex @article{li2023angle, title={AnglE-optimized
+Text Embeddings}, author={Li, Xianming and Li, Jing}, journal={arXiv preprint
+arXiv:2309.12871}, year={2023} } ``` # ð ChangeLogs | ð | Description |
+|----|------| | 2024 May 21 | support Espresso Sentence Embeddings | | 2024 Feb
+7 | support training with only positive pairs (`DatasetFormats.C`) | | 2023 Dec
+4 | Release a universal English sentence embedding model: [WhereIsAI/UAE-Large-
+V1](https://huggingface.co/WhereIsAI/UAE-Large-V1) | | 2023 Nov 2 | Release an
+English pretrained model: `SeanLee97/angle-llama-13b-nli` | | 2023 Oct 28 |
+Release two chinese pretrained models: `SeanLee97/angle-roberta-wwm-base-zhnli-
+v1` and `SeanLee97/angle-llama-7b-zhnli-v1`; Add chinese README.md | # ð§
+Contact If you have any questions or suggestions, please feel free to contact
+us via email: xmlee97@gmail.com # Â© License This project is licensed under the
+MIT License. For the pretrained models, please refer to the corresponding
+license of the models.
```

### Comparing `angle_emb-0.3.9/setup.py` & `angle_emb-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     requirements = [l for l in f.read().splitlines() if l]
 
 with open('dev-requirements.txt', encoding='utf-8') as f:
     test_requirements = [l for l in f.read().splitlines() if l][1:]
 
 setup(
     name='angle_emb',
-    version='0.3.9',
+    version='0.4.0',
     description='AnglE-optimize Text Embeddings',
     long_description=readme,
     long_description_content_type="text/markdown",
     author='sean lee',
     author_email='xmlee97@gmail.com',
     packages=find_packages(exclude=("tests", "tests.*", "examples", "examples.*")),
     install_requires=requirements,
@@ -38,11 +38,11 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     test_suite='tests',
     tests_require=test_requirements,
     entry_points={
         'console_scripts': [
-            'angle-trainer = angle_emb.train_cli:main',
+            'angle-trainer = angle_emb.angle_trainer:main',
         ],
     },
 )
```

