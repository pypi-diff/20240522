# Comparing `tmp/green-bit-llm-0.1.0.tar.gz` & `tmp/green-bit-llm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "green-bit-llm-0.1.0.tar", last modified: Wed May  1 10:53:36 2024, max compression
+gzip compressed data, was "green-bit-llm-0.2.0.tar", last modified: Wed May 22 21:36:24 2024, max compression
```

## Comparing `green-bit-llm-0.1.0.tar` & `green-bit-llm-0.2.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.982233 green-bit-llm-0.1.0/
--rw-r--r--   0 haojin     (501) staff       (20)    11357 2024-04-07 20:16:16.000000 green-bit-llm-0.1.0/LICENSE
--rw-r--r--   0 haojin     (501) staff       (20)     8583 2024-05-01 10:53:36.982076 green-bit-llm-0.1.0/PKG-INFO
--rw-r--r--   0 haojin     (501) staff       (20)     8219 2024-05-01 10:29:45.000000 green-bit-llm-0.1.0/README.md
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.976235 green-bit-llm-0.1.0/green_bit_llm/
--rw-r--r--   0 haojin     (501) staff       (20)       33 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)     1920 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/args_parser.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.977611 green-bit-llm-0.1.0/green_bit_llm/common/
--rw-r--r--   0 haojin     (501) staff       (20)       34 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/common/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)      156 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/common/enum.py
--rw-r--r--   0 haojin     (501) staff       (20)    17313 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/common/model.py
--rw-r--r--   0 haojin     (501) staff       (20)     6826 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/common/utils.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.978731 green-bit-llm-0.1.0/green_bit_llm/evaluation/
--rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/evaluation/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)     9588 2024-05-01 10:29:45.000000 green-bit-llm-0.1.0/green_bit_llm/evaluation/datautils.py
--rw-r--r--   0 haojin     (501) staff       (20)     7587 2024-05-01 10:29:45.000000 green-bit-llm-0.1.0/green_bit_llm/evaluation/evaluate.py
--rw-r--r--   0 haojin     (501) staff       (20)     4569 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/evaluation/lmclass.py
--rw-r--r--   0 haojin     (501) staff       (20)     2840 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/evaluation/utils.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.980034 green-bit-llm-0.1.0/green_bit_llm/inference/
--rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/inference/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)    21289 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/inference/chat_base.py
--rw-r--r--   0 haojin     (501) staff       (20)     5319 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/inference/chat_cli.py
--rw-r--r--   0 haojin     (501) staff       (20)    18476 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/inference/conversation.py
--rw-r--r--   0 haojin     (501) staff       (20)     4195 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/inference/sim_gen.py
--rw-r--r--   0 haojin     (501) staff       (20)     4536 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/inference/utils.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.980685 green-bit-llm-0.1.0/green_bit_llm/sft/
--rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)     4458 2024-05-01 10:29:45.000000 green-bit-llm-0.1.0/green_bit_llm/sft/finetune.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.981254 green-bit-llm-0.1.0/green_bit_llm/sft/optim/
--rw-r--r--   0 haojin     (501) staff       (20)       32 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/optim/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)     6259 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/optim/adamw8bit.py
--rw-r--r--   0 haojin     (501) staff       (20)    21387 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/optim/bnb_optimizer.py
--rw-r--r--   0 haojin     (501) staff       (20)     4160 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/peft_lora.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.981870 green-bit-llm-0.1.0/green_bit_llm/sft/peft_utils/
--rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/peft_utils/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)     9361 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/peft_utils/gba_lora.py
--rw-r--r--   0 haojin     (501) staff       (20)     2662 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/peft_utils/model.py
--rw-r--r--   0 haojin     (501) staff       (20)     5587 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/utils.py
--rw-r--r--   0 haojin     (501) staff       (20)       22 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/version.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.976835 green-bit-llm-0.1.0/green_bit_llm.egg-info/
--rw-r--r--   0 haojin     (501) staff       (20)     8583 2024-05-01 10:53:36.000000 green-bit-llm-0.1.0/green_bit_llm.egg-info/PKG-INFO
--rw-r--r--   0 haojin     (501) staff       (20)     1163 2024-05-01 10:53:36.000000 green-bit-llm-0.1.0/green_bit_llm.egg-info/SOURCES.txt
--rw-r--r--   0 haojin     (501) staff       (20)        1 2024-05-01 10:53:36.000000 green-bit-llm-0.1.0/green_bit_llm.egg-info/dependency_links.txt
--rw-r--r--   0 haojin     (501) staff       (20)      162 2024-05-01 10:53:36.000000 green-bit-llm-0.1.0/green_bit_llm.egg-info/requires.txt
--rw-r--r--   0 haojin     (501) staff       (20)       14 2024-05-01 10:53:36.000000 green-bit-llm-0.1.0/green_bit_llm.egg-info/top_level.txt
--rw-r--r--   0 haojin     (501) staff       (20)       38 2024-05-01 10:53:36.982281 green-bit-llm-0.1.0/setup.cfg
--rw-r--r--   0 haojin     (501) staff       (20)      865 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/setup.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.293589 green-bit-llm-0.2.0/
+-rw-r--r--   0 haojin     (501) staff       (20)    11357 2024-04-07 20:16:16.000000 green-bit-llm-0.2.0/LICENSE
+-rw-r--r--   0 haojin     (501) staff       (20)     9658 2024-05-22 21:36:24.291640 green-bit-llm-0.2.0/PKG-INFO
+-rw-r--r--   0 haojin     (501) staff       (20)     8889 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/README.md
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.281710 green-bit-llm-0.2.0/green_bit_llm/
+-rw-r--r--   0 haojin     (501) staff       (20)       33 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)     1920 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/args_parser.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.283052 green-bit-llm-0.2.0/green_bit_llm/common/
+-rw-r--r--   0 haojin     (501) staff       (20)       34 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/common/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)      156 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/common/enum.py
+-rw-r--r--   0 haojin     (501) staff       (20)    18420 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/green_bit_llm/common/model.py
+-rw-r--r--   0 haojin     (501) staff       (20)     8507 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/green_bit_llm/common/utils.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.284287 green-bit-llm-0.2.0/green_bit_llm/evaluation/
+-rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/evaluation/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)     9588 2024-05-01 10:29:45.000000 green-bit-llm-0.2.0/green_bit_llm/evaluation/datautils.py
+-rw-r--r--   0 haojin     (501) staff       (20)     8542 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/green_bit_llm/evaluation/evaluate.py
+-rw-r--r--   0 haojin     (501) staff       (20)     4569 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/evaluation/lmclass.py
+-rw-r--r--   0 haojin     (501) staff       (20)     2840 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/evaluation/utils.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.288579 green-bit-llm-0.2.0/green_bit_llm/inference/
+-rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/inference/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)    21289 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/inference/chat_base.py
+-rw-r--r--   0 haojin     (501) staff       (20)     5319 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/inference/chat_cli.py
+-rw-r--r--   0 haojin     (501) staff       (20)    18476 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/inference/conversation.py
+-rw-r--r--   0 haojin     (501) staff       (20)     4195 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/inference/sim_gen.py
+-rw-r--r--   0 haojin     (501) staff       (20)     4536 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/inference/utils.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.290049 green-bit-llm-0.2.0/green_bit_llm/sft/
+-rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/sft/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)     5110 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/green_bit_llm/sft/finetune.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.290768 green-bit-llm-0.2.0/green_bit_llm/sft/optim/
+-rw-r--r--   0 haojin     (501) staff       (20)       32 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/sft/optim/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)     6260 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/green_bit_llm/sft/optim/adamw8bit.py
+-rw-r--r--   0 haojin     (501) staff       (20)    21387 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/sft/optim/bnb_optimizer.py
+-rw-r--r--   0 haojin     (501) staff       (20)     4333 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/green_bit_llm/sft/peft_lora.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.291330 green-bit-llm-0.2.0/green_bit_llm/sft/peft_utils/
+-rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/sft/peft_utils/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)     9361 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/sft/peft_utils/gba_lora.py
+-rw-r--r--   0 haojin     (501) staff       (20)     2662 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/sft/peft_utils/model.py
+-rw-r--r--   0 haojin     (501) staff       (20)     2997 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/green_bit_llm/sft/trainer.py
+-rw-r--r--   0 haojin     (501) staff       (20)     5587 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/sft/utils.py
+-rw-r--r--   0 haojin     (501) staff       (20)       22 2024-05-22 21:36:20.000000 green-bit-llm-0.2.0/green_bit_llm/version.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.282267 green-bit-llm-0.2.0/green_bit_llm.egg-info/
+-rw-r--r--   0 haojin     (501) staff       (20)     9658 2024-05-22 21:36:24.000000 green-bit-llm-0.2.0/green_bit_llm.egg-info/PKG-INFO
+-rw-r--r--   0 haojin     (501) staff       (20)     1192 2024-05-22 21:36:24.000000 green-bit-llm-0.2.0/green_bit_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 haojin     (501) staff       (20)        1 2024-05-22 21:36:24.000000 green-bit-llm-0.2.0/green_bit_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 haojin     (501) staff       (20)      180 2024-05-22 21:36:24.000000 green-bit-llm-0.2.0/green_bit_llm.egg-info/requires.txt
+-rw-r--r--   0 haojin     (501) staff       (20)       14 2024-05-22 21:36:24.000000 green-bit-llm-0.2.0/green_bit_llm.egg-info/top_level.txt
+-rw-r--r--   0 haojin     (501) staff       (20)       38 2024-05-22 21:36:24.293639 green-bit-llm-0.2.0/setup.cfg
+-rw-r--r--   0 haojin     (501) staff       (20)      865 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/setup.py
```

### Comparing `green-bit-llm-0.1.0/LICENSE` & `green-bit-llm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.1.0/PKG-INFO` & `green-bit-llm-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: green-bit-llm
-Version: 0.1.0
-Summary: A toolkit for fine-tuning, inferencing, and evaluating GreenBitAI's LLMs.
-Home-page: https://github.com/GreenBitAI/green-bit-llm
-Author: GreenBitAI Contributors
-Author-email: team@greenbit.ai
-License: Apache-2.0
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Green-Bit-LLM
 
 A toolkit for fine-tuning, inferencing, and evaluating GreenBitAI's low-bit LLMs.
 
 ## Introduction
  
 This Python package uses the [Bitorch Engine](https://github.com/GreenBitAI/bitorch-engine) for efficient operations on [GreenBitAI's Low-bit Language Models (LLMs)](https://huggingface.co/GreenBitAI). 
@@ -24,14 +12,15 @@
 - [2024/04]
   - We have launched over **200 low-bit LLMs** in [GreenBitAI's Hugging Face Model Zoo](https://huggingface.co/GreenBitAI). Our release includes highly precise 2.2/2.5/3-bit models across the LLM family, featuring LLaMA 2/3, 01-Yi, Qwen, Mistral, Phi-3, Gemma, and more.
   - We released [Bitorch Engine](https://github.com/GreenBitAI/bitorch-engine) for **low-bit** quantized neural network operations. Our release support full parameter fine-tuning and parameter efficiency fine-tuning (PEFT), even under extremely constrained GPU resource conditions.
   - We released [gbx-lm](https://github.com/GreenBitAI/gbx-lm) python package which enables the efficient execution of [GreenBitAI's low-bit models](https://huggingface.co/collections/GreenBitAI/greenbitai-mlx-llm-6614eb6ceb8da657c2b4ed58) on Apple devices with [MLX](https://github.com/ml-explore/mlx).  
 
 ## LLMs
 
+We have released over 200 highly precise 2.2/2.5/3/4-bit models across the modern LLM family, featuring LLaMA 2/3, 01-Yi, Qwen, Mistral, Phi-3, and more. 
 
 |      Family      |        Bpw         |              Size              |                                                 HF collection_id                                                  |
 |:----------------:|:------------------:|:------------------------------:|:-----------------------------------------------------------------------------------------------------------------:|
 |     Llama-3      |  `4.0/3.0/2.5/2.2` |            `8B/70B`            | [`GreenBitAI Llama-3`](https://huggingface.co/collections/GreenBitAI/greenbitai-llama-3-6627bc1ec6538e3922c5d81c) |
 |     Llama-2      |   `3.0/2.5/2.2`    |          `7B/13B/70B`          | [`GreenBitAI Llama-2`](https://huggingface.co/collections/GreenBitAI/greenbitai-llama-2-661f87e3b073ff8e48a12834) |
 |     Qwen-1.5     | `4.0/3.0/2.5/2.2`  | `0.5B/1.8B/4B/7B/14B/32B/110B` | [`GreenBitAI Qwen 1.5`](https://huggingface.co/collections/GreenBitAI/greenbitai-qwen15-661f86ea69433f3d3062c920) |
 |      Phi-3       |   `3.0/2.5/2.2`    |             `mini`             |   [`GreenBitAI Phi-3`](https://huggingface.co/collections/GreenBitAI/greenbitai-phi-3-6628d008cdf168398a296c92)   |
@@ -39,14 +28,15 @@
 |      01-Yi       |   `3.0/2.5/2.2`    |            `6B/34B`            |   [`GreenBitAI 01-Yi`](https://huggingface.co/collections/GreenBitAI/greenbitai-01-yi-661f88af0648daa766d5102f)   |
 | Llama-3-instruct | `4.0/3.0/2.5/2.2`  |            `8B/70B`            | [`GreenBitAI Llama-3`](https://huggingface.co/collections/GreenBitAI/greenbitai-llama-3-6627bc1ec6538e3922c5d81c) |
 | Mistral-instruct |   `3.0/2.5/2.2`    |              `7B`              | [`GreenBitAI Mistral`](https://huggingface.co/collections/GreenBitAI/greenbitai-mistral-661f896c45da9d8b28a193a8) |                                                                                                                |
 |  Phi-3-instruct  |   `3.0/2.5/2.2`    |             `mini`             |   [`GreenBitAI Phi-3`](https://huggingface.co/collections/GreenBitAI/greenbitai-phi-3-6628d008cdf168398a296c92)   |
 |  Qwen-1.5-Chat   | `4.0/3.0/2.5/2.2`  | `0.5B/1.8B/4B/7B/14B/32B/110B` | [`GreenBitAI Qwen 1.5`](https://huggingface.co/collections/GreenBitAI/greenbitai-qwen15-661f86ea69433f3d3062c920) |
 |    01-Yi-Chat    |   `3.0/2.5/2.2`    |            `6B/34B`            |   [`GreenBitAI 01-Yi`](https://huggingface.co/collections/GreenBitAI/greenbitai-01-yi-661f88af0648daa766d5102f)   |           
 
+In addition to our low-bit models, green-bit-llm is fully compatible with the AutoGPTQ series of 4-bit quantization and compression models.
 
 ## Demo
 
 Full parameter fine-tuning of the LLaMA-3 8B model using a single GTX 3090 GPU with 24GB of graphics memory:
 
 <img src="assets/demo_llama3_8B_fpft.gif" width="960">
 
@@ -137,18 +127,24 @@
 ### Full-parameter fine-tuning
 
 Run the script as follows to fine-tune the quantized weights of the model on the target dataset. 
 The '--tune-qweight-only' parameter determines whether to fine-tune only the quantized weights or all weights, including non-quantized ones.
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python -m green_bit_llm.sft.finetune --model GreenBitAI/Qwen-1.5-1.8B-layer-mix-bpw-3.0 --dataset tatsu-lab/alpaca --optimizer DiodeMix --tune-qweight-only
+
+# AutoGPTQ model Q-SFT
+CUDA_VISIBLE_DEVICES=0 python -m green_bit_llm.sft.finetune --model astronomer/Llama-3-8B-Instruct-GPTQ-4-Bit --dataset tatsu-lab/alpaca --tune-qweight-only --batch-size 1
 ```
 
 ### Parameter efficient fine-tuning
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python -m green_bit_llm.sft.peft_lora --model GreenBitAI/Qwen-1.5-1.8B-layer-mix-bpw-3.0 --dataset tatsu-lab/alpaca --lr-fp 1e-6
+
+# AutoGPTQ model with Lora
+CUDA_VISIBLE_DEVICES=0 python -m green_bit_llm.sft.peft_lora --model astronomer/Llama-3-8B-Instruct-GPTQ-4-Bit --dataset tatsu-lab/alpaca --lr-fp 1e-6
 ```
 
 ## License
 We release our codes under the [Apache 2.0 License](LICENSE).
 Additionally, three packages are also partly based on third-party open-source codes. For detailed information, please refer to the description pages of the sub-projects.
```

### Comparing `green-bit-llm-0.1.0/README.md` & `green-bit-llm-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: green-bit-llm
+Version: 0.2.0
+Summary: A toolkit for fine-tuning, inferencing, and evaluating GreenBitAI's LLMs.
+Home-page: https://github.com/GreenBitAI/green-bit-llm
+Author: GreenBitAI Contributors
+Author-email: team@greenbit.ai
+License: Apache-2.0
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: accelerate>=0.27.2
+Requires-Dist: colorama
+Requires-Dist: datasets
+Requires-Dist: torch>=2.0.0
+Requires-Dist: sentencepiece
+Requires-Dist: transformers>=4.38.0
+Requires-Dist: huggingface-hub
+Requires-Dist: lm-eval==0.3.0
+Requires-Dist: termcolor
+Requires-Dist: pillow
+Requires-Dist: requests
+Requires-Dist: prompt-toolkit
+Requires-Dist: rich
+Requires-Dist: optimum
+Requires-Dist: auto-gptq
+
 # Green-Bit-LLM
 
 A toolkit for fine-tuning, inferencing, and evaluating GreenBitAI's low-bit LLMs.
 
 ## Introduction
  
 This Python package uses the [Bitorch Engine](https://github.com/GreenBitAI/bitorch-engine) for efficient operations on [GreenBitAI's Low-bit Language Models (LLMs)](https://huggingface.co/GreenBitAI). 
@@ -12,14 +39,15 @@
 - [2024/04]
   - We have launched over **200 low-bit LLMs** in [GreenBitAI's Hugging Face Model Zoo](https://huggingface.co/GreenBitAI). Our release includes highly precise 2.2/2.5/3-bit models across the LLM family, featuring LLaMA 2/3, 01-Yi, Qwen, Mistral, Phi-3, Gemma, and more.
   - We released [Bitorch Engine](https://github.com/GreenBitAI/bitorch-engine) for **low-bit** quantized neural network operations. Our release support full parameter fine-tuning and parameter efficiency fine-tuning (PEFT), even under extremely constrained GPU resource conditions.
   - We released [gbx-lm](https://github.com/GreenBitAI/gbx-lm) python package which enables the efficient execution of [GreenBitAI's low-bit models](https://huggingface.co/collections/GreenBitAI/greenbitai-mlx-llm-6614eb6ceb8da657c2b4ed58) on Apple devices with [MLX](https://github.com/ml-explore/mlx).  
 
 ## LLMs
 
+We have released over 200 highly precise 2.2/2.5/3/4-bit models across the modern LLM family, featuring LLaMA 2/3, 01-Yi, Qwen, Mistral, Phi-3, and more. 
 
 |      Family      |        Bpw         |              Size              |                                                 HF collection_id                                                  |
 |:----------------:|:------------------:|:------------------------------:|:-----------------------------------------------------------------------------------------------------------------:|
 |     Llama-3      |  `4.0/3.0/2.5/2.2` |            `8B/70B`            | [`GreenBitAI Llama-3`](https://huggingface.co/collections/GreenBitAI/greenbitai-llama-3-6627bc1ec6538e3922c5d81c) |
 |     Llama-2      |   `3.0/2.5/2.2`    |          `7B/13B/70B`          | [`GreenBitAI Llama-2`](https://huggingface.co/collections/GreenBitAI/greenbitai-llama-2-661f87e3b073ff8e48a12834) |
 |     Qwen-1.5     | `4.0/3.0/2.5/2.2`  | `0.5B/1.8B/4B/7B/14B/32B/110B` | [`GreenBitAI Qwen 1.5`](https://huggingface.co/collections/GreenBitAI/greenbitai-qwen15-661f86ea69433f3d3062c920) |
 |      Phi-3       |   `3.0/2.5/2.2`    |             `mini`             |   [`GreenBitAI Phi-3`](https://huggingface.co/collections/GreenBitAI/greenbitai-phi-3-6628d008cdf168398a296c92)   |
@@ -27,14 +55,15 @@
 |      01-Yi       |   `3.0/2.5/2.2`    |            `6B/34B`            |   [`GreenBitAI 01-Yi`](https://huggingface.co/collections/GreenBitAI/greenbitai-01-yi-661f88af0648daa766d5102f)   |
 | Llama-3-instruct | `4.0/3.0/2.5/2.2`  |            `8B/70B`            | [`GreenBitAI Llama-3`](https://huggingface.co/collections/GreenBitAI/greenbitai-llama-3-6627bc1ec6538e3922c5d81c) |
 | Mistral-instruct |   `3.0/2.5/2.2`    |              `7B`              | [`GreenBitAI Mistral`](https://huggingface.co/collections/GreenBitAI/greenbitai-mistral-661f896c45da9d8b28a193a8) |                                                                                                                |
 |  Phi-3-instruct  |   `3.0/2.5/2.2`    |             `mini`             |   [`GreenBitAI Phi-3`](https://huggingface.co/collections/GreenBitAI/greenbitai-phi-3-6628d008cdf168398a296c92)   |
 |  Qwen-1.5-Chat   | `4.0/3.0/2.5/2.2`  | `0.5B/1.8B/4B/7B/14B/32B/110B` | [`GreenBitAI Qwen 1.5`](https://huggingface.co/collections/GreenBitAI/greenbitai-qwen15-661f86ea69433f3d3062c920) |
 |    01-Yi-Chat    |   `3.0/2.5/2.2`    |            `6B/34B`            |   [`GreenBitAI 01-Yi`](https://huggingface.co/collections/GreenBitAI/greenbitai-01-yi-661f88af0648daa766d5102f)   |           
 
+In addition to our low-bit models, green-bit-llm is fully compatible with the AutoGPTQ series of 4-bit quantization and compression models.
 
 ## Demo
 
 Full parameter fine-tuning of the LLaMA-3 8B model using a single GTX 3090 GPU with 24GB of graphics memory:
 
 <img src="assets/demo_llama3_8B_fpft.gif" width="960">
 
@@ -125,18 +154,24 @@
 ### Full-parameter fine-tuning
 
 Run the script as follows to fine-tune the quantized weights of the model on the target dataset. 
 The '--tune-qweight-only' parameter determines whether to fine-tune only the quantized weights or all weights, including non-quantized ones.
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python -m green_bit_llm.sft.finetune --model GreenBitAI/Qwen-1.5-1.8B-layer-mix-bpw-3.0 --dataset tatsu-lab/alpaca --optimizer DiodeMix --tune-qweight-only
+
+# AutoGPTQ model Q-SFT
+CUDA_VISIBLE_DEVICES=0 python -m green_bit_llm.sft.finetune --model astronomer/Llama-3-8B-Instruct-GPTQ-4-Bit --dataset tatsu-lab/alpaca --tune-qweight-only --batch-size 1
 ```
 
 ### Parameter efficient fine-tuning
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python -m green_bit_llm.sft.peft_lora --model GreenBitAI/Qwen-1.5-1.8B-layer-mix-bpw-3.0 --dataset tatsu-lab/alpaca --lr-fp 1e-6
+
+# AutoGPTQ model with Lora
+CUDA_VISIBLE_DEVICES=0 python -m green_bit_llm.sft.peft_lora --model astronomer/Llama-3-8B-Instruct-GPTQ-4-Bit --dataset tatsu-lab/alpaca --lr-fp 1e-6
 ```
 
 ## License
 We release our codes under the [Apache 2.0 License](LICENSE).
 Additionally, three packages are also partly based on third-party open-source codes. For detailed information, please refer to the description pages of the sub-projects.
```

### Comparing `green-bit-llm-0.1.0/green_bit_llm/args_parser.py` & `green-bit-llm-0.2.0/green_bit_llm/args_parser.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.1.0/green_bit_llm/common/model.py` & `green-bit-llm-0.2.0/green_bit_llm/common/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 from pathlib import Path
 from typing import Optional, Tuple, Dict
 import json
+import os
 
 import torch
 import torch.nn as nn
 
 from transformers import PreTrainedTokenizer, AutoTokenizer, AutoConfig, AutoModelForCausalLM, PreTrainedModel, logging
 import accelerate
+from auto_gptq.nn_modules.qlinear.qlinear_cuda import QuantLinear
 
-from .utils import get_layer_mode_from_name, get_packed_info, get_model_path, find_layers, apply_dtype_to
+from .utils import get_layer_mode, get_packed_info, get_model_path, find_layers, apply_dtype_to
+from .utils import STRATEGY_FILE_NAME, MODEL_TYPE_QWEN2, STRATEGY_FILE_JSON_ROOT
 from .enum import LayerMode, TextGenMode
 
 import time
-from transformers import logging
 
 ENGINE_AVAILABLE = True
 try:
     from bitorch_engine.layers.qlinear.nbit import MPQLinearBase
     from bitorch_engine.layers.qlinear.nbit.cuda import MPQLinearCuda, MBWQLinearCuda
 except ModuleNotFoundError as e:
     ENGINE_AVAILABLE = False
     print(f"Error: Module not found: {e}.")
 
 from colorama import init, Fore, Style
 init(autoreset=True)
 
-STRATEGY_FILE_NAME = "quant_strategy.json"
-MODEL_TYPE_QWEN2 = "qwen2"
-STRATEGY_FILE_JSON_ROOT = "measurement"
-
 
 def engine_layer_prepare(model: torch.nn.Module):
     """
     Define the function that prepares the engine layer.
 
     Args:
         model (nn.Module): The PyTorch module will be operated.
@@ -101,18 +99,26 @@
             if strategy:
                 groups, rows = get_packed_info(tmp.in_features, strategy["bits"], strategy["bits_prop"], strategy["group_size"])
                 bits = strategy["bits"][0]
                 group_size = strategy["group_size"][str(bits)]
 
             disable_bias = get_disable_bias(name_attr, model_type)
 
+            # Check if auto_gptq.QuantLinear is used
+            is_quant_linear = isinstance(tmp, QuantLinear)
+            use_gba_quant = not is_quant_linear
+            asym = is_quant_linear
+            in_c = tmp.infeatures if is_quant_linear else tmp.in_features
+            out_c = tmp.outfeatures if is_quant_linear else tmp.out_features
+
             common_params = {
-                "in_channels": tmp.in_features, "out_channels": tmp.out_features,
+                "in_channels": in_c,
+                "out_channels": out_c,
                 "w_bit": bits, "dtype": dtype, "group_size": group_size, "dq_group_size": 32,
-                "use_gba_quant": True, "asym": False, "dq_mode": 2, "requires_grad": requires_grad,
+                "use_gba_quant": use_gba_quant, "asym": asym, "dq_mode": 2, "requires_grad": requires_grad,
                 "disable_bias": disable_bias
             }
 
             if layer_mode == LayerMode.LEGENCY:
                 quantized_layer = MPQLinearCuda(**common_params)
             elif layer_mode == LayerMode.LAYER_MIX:
                 quantized_layer = MBWQLinearCuda(use_mbw=False, **common_params)
@@ -124,55 +130,74 @@
             setattr(module, attr, quantized_layer)
 
     for name_attr, child in module.named_children():
         name_sub = f'{name}.{name_attr}' if name else name_attr
         make_quant(child, names, layer_mode, name_sub, group_size, bits, dtype, quant_strategy, model_type, requires_grad)
 
 
-def load_model(model_path: Path, layer_mode: LayerMode, bits: Optional[int] = None, group_size: Optional[int] = None,
+def load_strategy_file(model_path: Path, layer_mode: LayerMode) -> Dict:
+    """
+        Load strategy configuration from a file based on the provided layer mode.
+
+        Args:
+            model_path (Path): The file system path to the model directory.
+            layer_mode (LayerMode): The mode of the layers, either 'layer_mix' or 'channel_mix'.
+
+        Returns:
+            Dict: A dictionary containing the strategy configuration if the layer_mode is
+                  'layer_mix' or 'channel_mix'. Returns an empty dictionary otherwise.
+
+        Raises:
+            FileNotFoundError: If the strategy configuration file is not found in the specified path.
+    """
+    strategy = {}
+    if layer_mode in (LayerMode.LAYER_MIX, LayerMode.CHANNEL_MIX):
+        strategy_path = os.path.join(model_path, STRATEGY_FILE_NAME)
+        try:
+            with open(strategy_path, "r") as file:
+                strategy = json.load(file)[STRATEGY_FILE_JSON_ROOT]
+        except FileNotFoundError:
+            raise FileNotFoundError(f"Error: Strategy config file not found in {model_path}")
+    return strategy
+
+
+def load_model(model_path: Path, config: AutoConfig, layer_mode: LayerMode, bits: Optional[int] = None, group_size: Optional[int] = None,
                dtype: torch.dtype = torch.half, device_map: set = {"cuda:0"}, seqlen: int = 2048,
-               model_config: Dict = {}, requires_grad: bool = False) -> Tuple[nn.Module, AutoConfig]:
+               model_config: Dict = {}, requires_grad: bool = False) -> nn.Module:
     """
     Load and initialize a model from the given path with options for quantization and device distribution.
 
     This function loads a model, applies quantization based on the provided layer mode, bits, and group size,
     and distributes the model across specified devices. It returns both the model and its configuration.
 
     Args:
         model_path (Path): Path to the model.
+        config (Dict): configs loaded from hf-model-config.
         layer_mode (LayerMode): Layer mode for quantization.
         bits (Optional[int]): Number of bits for quantization.
         group_size (Optional[int]): Group size for quantization.
         dtype (torch.dtype): Data type for model tensors.
         device_map (set): Devices to distribute the model.
         seqlen (int): Sequence length for the model.
         model_config (str, optional): Model configurations for "AutoModelForCausalLM.from_pretrained".
         requires_grad (bool): Set if the model requires gradient. It can be set to True for training.
 
     Returns:
-        Tuple[nn.Module, AutoConfig]: A tuple containing the loaded and initialized model and its configuration.
+        nn.Module: The loaded and initialized model.
     """
     logging.set_verbosity_error()
 
     start_time = time.time()
     print(Style.BRIGHT + Fore.CYAN + "Info: Loading Model ...")
 
     # Load quantization strategy if applicable
-    strategy = {}
-    if layer_mode in (LayerMode.LAYER_MIX, LayerMode.CHANNEL_MIX):
-        strategy_path = model_path / STRATEGY_FILE_NAME
-        try:
-            with open(strategy_path, "r") as file:
-                strategy = json.load(file)[STRATEGY_FILE_JSON_ROOT]
-        except FileNotFoundError:
-            raise FileNotFoundError(f"Error: Strategy config file not found in {model_path}")
+    strategy = load_strategy_file(model_path, layer_mode)
 
     # Initialize model with empty weights and load configuration
     with accelerate.init_empty_weights():
-        config = AutoConfig.from_pretrained(model_path, trust_remote_code=True)
         model = AutoModelForCausalLM.from_pretrained(model_path, config=config, torch_dtype=dtype, **model_config).eval()
 
         # Quantize layers as necessary
         for i, layer in enumerate(model.model.layers):
             layers = find_layers(layer)
             layers_to_quantize = {name: layer for name, layer in layers.items() if name != 'lm_head'}
 
@@ -188,15 +213,15 @@
     engine_layer_prepare(model)  # Assuming this prepares the model's engine layers post-initialization
     apply_dtype_to(model, dtype)  # Assuming this function applies the dtype to all model parameters
 
     print(Style.BRIGHT + Fore.CYAN + f"Info: Apply dtype: {dtype} to the model.")
     print(Style.BRIGHT + Fore.CYAN + f'Info: Total {torch.cuda.memory_allocated() / 1024**3:.2f} GiB VRAM used.')
     print(Style.BRIGHT + Fore.CYAN + f"Info: Loaded the model in {time.time() - start_time:.2f} seconds.")
 
-    return model, config
+    return model
 
 
 def load(
     path_or_hf_repo: str,
     tokenizer_config: Dict = {},
     dtype: torch.dtype = torch.half,
     device_map: set = {"cuda:0"},
@@ -224,18 +249,21 @@
         FileNotFoundError: If the config file or safetensors are not found.
         ValueError: If the model class or args class are not found.
         NotImplementedError: If the LoRA layers functionality is not implemented.
     """
     if not ENGINE_AVAILABLE:
         raise Exception("Error: Bitorch Engine layers are not available.")
 
-    layer_mode, bits, group_size = get_layer_mode_from_name(path_or_hf_repo)
     model_path = get_model_path(path_or_hf_repo)
 
-    model, config = load_model(model_path, layer_mode, bits, group_size, dtype, device_map, seqlen, model_config, requires_grad)
+    config = AutoConfig.from_pretrained(model_path, trust_remote_code=True)
+
+    layer_mode, bits, group_size = get_layer_mode(path_or_hf_repo, config)
+
+    model = load_model(model_path, config, layer_mode, bits, group_size, dtype, device_map, seqlen, model_config, requires_grad)
 
     tokenizer = AutoTokenizer.from_pretrained(path_or_hf_repo, **tokenizer_config)
 
     return model, tokenizer, config
 
 
 def generate(
```

### Comparing `green-bit-llm-0.1.0/green_bit_llm/evaluation/datautils.py` & `green-bit-llm-0.2.0/green_bit_llm/evaluation/datautils.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.1.0/green_bit_llm/evaluation/evaluate.py` & `green-bit-llm-0.2.0/green_bit_llm/evaluation/evaluate.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,40 @@
 import sys
 
 import torch
 import torch.nn as nn
 
 from tqdm import tqdm
 
+import safetensors
+from peft import PeftModel, LoraConfig, get_peft_model
+
 from .lmclass import LMClass
 from .utils import create_logger, add_dict_to_json_file
 from .datautils import get_loaders
 
 from green_bit_llm.common import load
+from green_bit_llm.common.utils import get_model_path
+from green_bit_llm.sft.peft_utils.model import *
+from peft import PeftModel, LoraConfig, get_peft_model
 from pathlib import Path
  
 from lm_eval import evaluator
 
 import warnings
 
 warnings.filterwarnings('ignore')
 
 # default value for arguments
 DEFAULT_MODEL_PATH = "GreenBitAI/Qwen-1.5-1.8B-layer-mix-bpw-2.2"
 DEFAULT_SEQLEN = 2048
 DEFAULT_RANDOM_SEED = 0
 DTYPE = torch.half
 
+replace_peft_lora_model_with_gba_lora_model()
 
 @torch.no_grad()
 def lm_evaluate(lm, args, logger):
     """
     Evaluates the language model (lm) according to the specified evaluation parameters in args.
     This function handles both perplexity evaluation on various datasets and few-shot learning evaluation.
 
@@ -51,15 +58,19 @@
             dataloader, testloader = get_loaders(
                 dataset,
                 seed=args.seed,
                 model=args.model,
                 seqlen=args.seqlen,
             )
             
-            testenc = testloader
+            if "c4" in dataset:
+                testenc = testloader
+            else:
+                testenc = testloader.input_ids
+
             nsamples = testenc.numel() // lm.seqlen
             use_cache = lm.model.config.use_cache
             lm.model.config.use_cache = False
             lm.model.eval()
             nlls = []
             
             for i in tqdm(range(nsamples)):
@@ -166,29 +177,36 @@
         type=int,
         default=0,
         help="Specify num of few shot examples for evaluation.",
     )
     parser.add_argument(
         "--few-shot-tasks",
         type=str,
-        default="openbookqa,arc_easy,winogrande,hellaswag,arc_challenge,piqa,boolq,race,truthfulqa_mc,anli_r1,anli_r2,anli_r3,wic",
+        default="openbookqa,arc_easy,winogrande,hellaswag,arc_challenge,piqa,boolq,race,anli_r1,anli_r2,anli_r3,wic",
         help="Few-shot learning ability evaluation tasks.",
     )
     parser.add_argument(
         "--batch-size",
         type=int,
         default=16,
         help="Batch size for few-shot evaluation.",
     )
     parser.add_argument(
         "--save-dir",
         type=str,
         default="log/",
         help="Specify save dir for eval results.",
     )
+    parser.add_argument(
+        "--lora-dir",
+        type=str,
+        default=None,
+        help="Specify lora dir for lora merge"
+
+    )
     return parser
 
 
 def create_device_map(cuda_device_id):
     ids = cuda_device_id.split(',')
     # Create strings in the format "cuda:x" for each ID and put them into the collection
     device_map = {f"cuda:{id}" for id in ids}
@@ -203,36 +221,48 @@
     pretrain_model_config = {
         "trust_remote_code": True if args.trust_remote_code else None,
         "use_flash_attention_2": True if args.use_flash_attention_2 else None
     }
 
     if args.eos_token is not None:
         tokenizer_config["eos_token"] = args.eos_token
-
+    
     model, tokenizer, config = load(
         args.model,
         tokenizer_config=tokenizer_config,
         dtype=DTYPE,
         device_map='auto',
         seqlen=args.seqlen,
         model_config=pretrain_model_config,
         requires_grad=False
     )
-
+    
+    if args.lora_dir is not None:
+        config = LoraConfig(
+            r=64,
+            lora_alpha=32,
+            target_modules=["q_proj", "v_proj", "out_proj", "up_proj"],
+            lora_dropout=0.01,
+            bias="none",
+            task_type="CAUSAL_LM",
+        )
+        model = get_peft_model(model,config)
+        model.load_adapter(args.lora_dir, adapter_name="default")
 
     lm = LMClass(args.model, batch_size=args.batch_size, config=config, tokenizer=tokenizer, model=model)
     lm.seqlen = args.seqlen
     
     logger = create_logger(Path(args.save_dir))
-
-    eval_results = lm_evaluate(lm=lm, args=args, logger=logger)
+    
+    with torch.no_grad():
+        eval_results = lm_evaluate(lm=lm, args=args, logger=logger)
 
     eval_results = {"{}".format(args.model): eval_results}
 
-    add_dict_to_json_file(file_path="{}".format(args.save_dir + "eval_results.json"), new_data=eval_results)
+    add_dict_to_json_file(file_path="{}".format(os.path.join(args.save_dir, "eval_results.json")), new_data=eval_results)
 
 if __name__ == "__main__":
     if not torch.cuda.is_available():
         print("Warning: CUDA is needed to run the model.")
         sys.exit(0)
 
     parser = setup_arg_parser()
```

### Comparing `green-bit-llm-0.1.0/green_bit_llm/evaluation/lmclass.py` & `green-bit-llm-0.2.0/green_bit_llm/evaluation/lmclass.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.1.0/green_bit_llm/evaluation/utils.py` & `green-bit-llm-0.2.0/green_bit_llm/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.1.0/green_bit_llm/inference/chat_base.py` & `green-bit-llm-0.2.0/green_bit_llm/inference/chat_base.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.1.0/green_bit_llm/inference/chat_cli.py` & `green-bit-llm-0.2.0/green_bit_llm/inference/chat_cli.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.1.0/green_bit_llm/inference/conversation.py` & `green-bit-llm-0.2.0/green_bit_llm/inference/conversation.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.1.0/green_bit_llm/inference/sim_gen.py` & `green-bit-llm-0.2.0/green_bit_llm/inference/sim_gen.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.1.0/green_bit_llm/inference/utils.py` & `green-bit-llm-0.2.0/green_bit_llm/inference/utils.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.1.0/green_bit_llm/sft/finetune.py` & `green-bit-llm-0.2.0/green_bit_llm/sft/peft_lora.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,88 +1,62 @@
-import argparse
+import os
 import sys
 
 import torch
 
 from transformers import PreTrainedTokenizer, TrainingArguments
 from datasets import load_dataset
-from trl import SFTTrainer
+from .trainer import GbaSFTTrainer
+from peft import PeftModel, LoraConfig, get_peft_model
 
 from green_bit_llm.common import load
 from green_bit_llm.args_parser import setup_shared_arg_parser
 
-import warnings
+from .peft_utils.model import *
+from .optim import AdamW8bit
 
+import warnings
 warnings.filterwarnings('ignore')
 
 try:
     from bitorch_engine.optim import DiodeMix
-    from bitorch_engine.layers.qlinear.nbit import MPQLinearBase
 except ModuleNotFoundError as e:
     raise Exception(f"Error occurred while importing Bitorch Engine module '{str(e)}'.")
 
-from .optim import AdamW8bit
-
 from .utils import str_to_torch_dtype, create_param_groups
 
-
 # default value for arguments
 DEFAULT_MODEL_PATH = "GreenBitAI/Qwen-1.5-1.8B-layer-mix-bpw-3.0"
 DEFAULT_SEQLEN = 512
 DEFAULT_RANDOM_SEED = 0
 DEFAULT_LR = 1e-5
 DEFAULT_LR_GALORE = 1e-4
-DEFAULT_LR_ADAMW8BIT = 5e-3
-DEFAULT_BETAS = (0.95, 0.999)
+DEFAULT_LR_FP = 1e-6
+DEFAULT_BETAS = (0.9, 0.999)
 
 
 def setup_arg_parser():
     """Set up and return the argument parser."""
-    parser = setup_shared_arg_parser("green-bit-llm finetune script")
+    parser = setup_shared_arg_parser("green-bit-llm lora script")
     parser.add_argument(
         "--seed",
         type=int,
         default=DEFAULT_RANDOM_SEED,
         help="The random seed for data loader.",
     )
-    # GaLore parameters
-    parser.add_argument(
-        "--galore",
-        action="store_true",
-        help="Enable using galore",
-    )
-    parser.add_argument("--galore-rank", type=int, default=128)
-    parser.add_argument("--galore-update-proj-gap", type=int, default=200)
-    parser.add_argument("--galore-scale", type=float, default=0.25)
-    parser.add_argument("--galore-proj-type", type=str, default="std")
-
     # qweight related
     parser.add_argument(
-        "--tune-qweight-only",
-        action="store_true",
-        help="Set whether to adjust only the low-bit qweight and keep the regular parameters unchanged during the training process.",
-    )
-    parser.add_argument(
-        "--lr-2bit",
-        type=float,
-        default=-1.0,
-        help="Learning rate for 2-bit qweight."
-    )
-    parser.add_argument(
-        "--lr-4bit",
-        type=float,
-        default=-1.0,
-        help="Learning rate for 4-bit qweight."
-    )
-    parser.add_argument(
         "--lr-fp",
         type=float,
-        default=DEFAULT_LR,
+        default=DEFAULT_LR_FP,
         help="Learning rate for full-precision weight."
     )
+    parser.add_argument("--lora-rank", type=int, default=64)
+    parser.add_argument("--lora-alpha", type=int, default=32)
+    parser.add_argument("--lora-dropout", type=float, default=0.01)
     return parser
 
 
 def main(args):
 
     # Building configs
     tokenizer_config = {"trust_remote_code": True if args.trust_remote_code else None}
@@ -93,60 +67,78 @@
 
     model, tokenizer, config = load(
         args.model,
         tokenizer_config=tokenizer_config,
         device_map='auto',
         seqlen=args.seqlen,
         model_config=pretrain_model_config,
-        requires_grad=True,
+        requires_grad=False,
     )
+    
+    config = LoraConfig(
+        r=args.lora_rank,
+        lora_alpha=args.lora_alpha,
+        target_modules=["q_proj", "v_proj", "out_proj", "down_proj", "up_proj"],
+        lora_dropout=args.lora_dropout,
+        bias="none",
+        task_type="CAUSAL_LM",
+    )
+    
+    replace_peft_lora_model_with_gba_lora_model()
+
+    model = get_peft_model(model, config)
 
-    param_groups = create_param_groups(model, args, DEFAULT_BETAS, DEFAULT_LR_GALORE, DEFAULT_LR_ADAMW8BIT, DEFAULT_LR)
+    param_groups = create_param_groups(model, args, DEFAULT_BETAS)
 
     model.train()
 
     dataset = load_dataset(args.dataset, split="train")
     
-    args.save_dir = args.save_dir + args.model
+    args.save_dir = os.path.join(args.save_dir, "lora/", args.model)
 
     train_args = TrainingArguments(
                     output_dir=args.save_dir,
                     gradient_checkpointing=True,
-                    # auto_find_batch_size=True,
+                    #auto_find_batch_size=True,
                     per_device_train_batch_size=args.batch_size,
                     logging_steps=1,
+                    num_train_epochs=1,
+                    gradient_accumulation_steps=1,
                     save_steps=args.save_step,
+                    #warmup_ratio=0.05,
                     max_grad_norm=0, # NOTE: max_grad_norm MUST be <= 0 or None, otherwise raise dtype error due to the Int dtype of qweight.
                 )
 
     # Optimizer
     if 'adamw8bit' in args.optimizer.lower():
-        optimizer = AdamW8bit(param_groups, weight_decay=args.weight_decay, dtype=str_to_torch_dtype(args.dtype))
+        optimizer = AdamW8bit(param_groups, weight_decay=args.weight_decay, lr=5e-3, dtype=str_to_torch_dtype(args.dtype))
     elif 'diodemix' in args.optimizer.lower():
         optimizer = DiodeMix(param_groups, dtype=str_to_torch_dtype(args.dtype))
-
     optimizers = (optimizer, None)
-
-    # Trainer
-    trainer = SFTTrainer(
+    
+    for name, param in model.named_parameters():
+        if "qweight" not in name:
+            param.requires_grad = True
+    
+    trainer = GbaSFTTrainer(
         model=model,
         args=train_args,
         train_dataset=dataset,
         dataset_text_field="text",
         optimizers=optimizers,
         max_seq_length=args.seqlen,
     )
-
+    
     trainer.train()
 
     model.save_pretrained(args.save_dir)
 
 
 if __name__ == "__main__":
     if not torch.cuda.is_available():
-        print("Warning: CUDA is required to run the model.")
+        print("Warning: CUDA is needed to run the model.")
         sys.exit(0)
 
     parser = setup_arg_parser()
     args = parser.parse_args()
 
     main(args)
```

### Comparing `green-bit-llm-0.1.0/green_bit_llm/sft/optim/adamw8bit.py` & `green-bit-llm-0.2.0/green_bit_llm/sft/optim/adamw8bit.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 try:
     from galore_torch.galore_projector import GaLoreProjector
 except ModuleNotFoundError as e:
     raise Exception("Error: GaLoreProjector is not available. Make sure 'galore-torch' has been installed on you system.")
 
 try:
     from bitorch_engine.layers.qlinear.nbit import MPQWeightParameter
-    from bitorch_engine.utils.quant_operators import gptq_stype_unpacking
+    from bitorch_engine.utils.quant_operators import gptq_style_unpacking
     from bitorch_engine.layers.qlinear.nbit.cuda.utils import pack_fp_weight
 except ModuleNotFoundError as e:
     raise Exception(f"Error occurred while importing Bitorch Engine module '{str(e)}'.")
 
 
 class AdamW8bit(Optimizer2State):
     def __init__(self, params, lr=1e-3, betas=(0.9, 0.999), eps=1e-8, weight_decay=.0, amsgrad=False, optim_bits=8,
@@ -97,30 +97,30 @@
                 if "rank" in group:
                     # now the p.data is actually: -norm_grad*lr
                     norm_grad = projector.project_back(p.data)
 
                     if isinstance(p, MPQWeightParameter):
                         # unpack qweight
                         p.data = saved_data
-                        w_unpacked = gptq_stype_unpacking(p).to(self.dtype).to(saved_data.device)
+                        w_unpacked = gptq_style_unpacking(p).to(self.dtype).to(saved_data.device)
                         w_unpacked.add_(norm_grad)
                         if group["weight_decay"] > 0.0:
                             w_unpacked.add_(w_unpacked, alpha=-group['lr'] * group['weight_decay'])
                         # pack fp weight back to Q-weight and update qweight data
                         p.data = pack_fp_weight(w_unpacked, p)
                     else:
                         p.data = saved_data.add_(norm_grad)
                         if group["weight_decay"] > 0.0:
                             p.data.add_(p.data, alpha=-group['lr'] * group['weight_decay'])
                 elif isinstance(p, MPQWeightParameter):
                     # now the p.data is actually: -norm_grad*lr
                     norm_grad = p.data.clone()
                     # unpack qweight
                     p.data = saved_data
-                    w_unpacked = gptq_stype_unpacking(p).to(self.dtype).to(saved_data.device)
+                    w_unpacked = gptq_style_unpacking(p).to(self.dtype).to(saved_data.device)
                     w_unpacked.add_(norm_grad)
                     if group["weight_decay"] > 0.0:
                         w_unpacked.add_(w_unpacked, alpha=-group['lr'] * group['weight_decay'])
                     # pack fp weight back to Q-weight and update qweight data
                     p.data = pack_fp_weight(w_unpacked, p)
 
                 # pack fp weight back to qweight
@@ -132,8 +132,8 @@
                     torch.cuda.empty_cache()
 
         if self.is_paged:
             # all paged operation are asynchronous, we need
             # to sync to make sure all tensors are in the right state
             torch.cuda.synchronize()
 
-        return loss
+        return loss
```

### Comparing `green-bit-llm-0.1.0/green_bit_llm/sft/optim/bnb_optimizer.py` & `green-bit-llm-0.2.0/green_bit_llm/sft/optim/bnb_optimizer.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.1.0/green_bit_llm/sft/peft_utils/gba_lora.py` & `green-bit-llm-0.2.0/green_bit_llm/sft/peft_utils/gba_lora.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.1.0/green_bit_llm/sft/peft_utils/model.py` & `green-bit-llm-0.2.0/green_bit_llm/sft/peft_utils/model.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.1.0/green_bit_llm/sft/utils.py` & `green-bit-llm-0.2.0/green_bit_llm/sft/utils.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.1.0/green_bit_llm.egg-info/PKG-INFO` & `green-bit-llm-0.2.0/green_bit_llm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,33 @@
 Metadata-Version: 2.1
 Name: green-bit-llm
-Version: 0.1.0
+Version: 0.2.0
 Summary: A toolkit for fine-tuning, inferencing, and evaluating GreenBitAI's LLMs.
 Home-page: https://github.com/GreenBitAI/green-bit-llm
 Author: GreenBitAI Contributors
 Author-email: team@greenbit.ai
 License: Apache-2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: accelerate>=0.27.2
+Requires-Dist: colorama
+Requires-Dist: datasets
+Requires-Dist: torch>=2.0.0
+Requires-Dist: sentencepiece
+Requires-Dist: transformers>=4.38.0
+Requires-Dist: huggingface-hub
+Requires-Dist: lm-eval==0.3.0
+Requires-Dist: termcolor
+Requires-Dist: pillow
+Requires-Dist: requests
+Requires-Dist: prompt-toolkit
+Requires-Dist: rich
+Requires-Dist: optimum
+Requires-Dist: auto-gptq
 
 # Green-Bit-LLM
 
 A toolkit for fine-tuning, inferencing, and evaluating GreenBitAI's low-bit LLMs.
 
 ## Introduction
  
@@ -24,14 +39,15 @@
 - [2024/04]
   - We have launched over **200 low-bit LLMs** in [GreenBitAI's Hugging Face Model Zoo](https://huggingface.co/GreenBitAI). Our release includes highly precise 2.2/2.5/3-bit models across the LLM family, featuring LLaMA 2/3, 01-Yi, Qwen, Mistral, Phi-3, Gemma, and more.
   - We released [Bitorch Engine](https://github.com/GreenBitAI/bitorch-engine) for **low-bit** quantized neural network operations. Our release support full parameter fine-tuning and parameter efficiency fine-tuning (PEFT), even under extremely constrained GPU resource conditions.
   - We released [gbx-lm](https://github.com/GreenBitAI/gbx-lm) python package which enables the efficient execution of [GreenBitAI's low-bit models](https://huggingface.co/collections/GreenBitAI/greenbitai-mlx-llm-6614eb6ceb8da657c2b4ed58) on Apple devices with [MLX](https://github.com/ml-explore/mlx).  
 
 ## LLMs
 
+We have released over 200 highly precise 2.2/2.5/3/4-bit models across the modern LLM family, featuring LLaMA 2/3, 01-Yi, Qwen, Mistral, Phi-3, and more. 
 
 |      Family      |        Bpw         |              Size              |                                                 HF collection_id                                                  |
 |:----------------:|:------------------:|:------------------------------:|:-----------------------------------------------------------------------------------------------------------------:|
 |     Llama-3      |  `4.0/3.0/2.5/2.2` |            `8B/70B`            | [`GreenBitAI Llama-3`](https://huggingface.co/collections/GreenBitAI/greenbitai-llama-3-6627bc1ec6538e3922c5d81c) |
 |     Llama-2      |   `3.0/2.5/2.2`    |          `7B/13B/70B`          | [`GreenBitAI Llama-2`](https://huggingface.co/collections/GreenBitAI/greenbitai-llama-2-661f87e3b073ff8e48a12834) |
 |     Qwen-1.5     | `4.0/3.0/2.5/2.2`  | `0.5B/1.8B/4B/7B/14B/32B/110B` | [`GreenBitAI Qwen 1.5`](https://huggingface.co/collections/GreenBitAI/greenbitai-qwen15-661f86ea69433f3d3062c920) |
 |      Phi-3       |   `3.0/2.5/2.2`    |             `mini`             |   [`GreenBitAI Phi-3`](https://huggingface.co/collections/GreenBitAI/greenbitai-phi-3-6628d008cdf168398a296c92)   |
@@ -39,14 +55,15 @@
 |      01-Yi       |   `3.0/2.5/2.2`    |            `6B/34B`            |   [`GreenBitAI 01-Yi`](https://huggingface.co/collections/GreenBitAI/greenbitai-01-yi-661f88af0648daa766d5102f)   |
 | Llama-3-instruct | `4.0/3.0/2.5/2.2`  |            `8B/70B`            | [`GreenBitAI Llama-3`](https://huggingface.co/collections/GreenBitAI/greenbitai-llama-3-6627bc1ec6538e3922c5d81c) |
 | Mistral-instruct |   `3.0/2.5/2.2`    |              `7B`              | [`GreenBitAI Mistral`](https://huggingface.co/collections/GreenBitAI/greenbitai-mistral-661f896c45da9d8b28a193a8) |                                                                                                                |
 |  Phi-3-instruct  |   `3.0/2.5/2.2`    |             `mini`             |   [`GreenBitAI Phi-3`](https://huggingface.co/collections/GreenBitAI/greenbitai-phi-3-6628d008cdf168398a296c92)   |
 |  Qwen-1.5-Chat   | `4.0/3.0/2.5/2.2`  | `0.5B/1.8B/4B/7B/14B/32B/110B` | [`GreenBitAI Qwen 1.5`](https://huggingface.co/collections/GreenBitAI/greenbitai-qwen15-661f86ea69433f3d3062c920) |
 |    01-Yi-Chat    |   `3.0/2.5/2.2`    |            `6B/34B`            |   [`GreenBitAI 01-Yi`](https://huggingface.co/collections/GreenBitAI/greenbitai-01-yi-661f88af0648daa766d5102f)   |           
 
+In addition to our low-bit models, green-bit-llm is fully compatible with the AutoGPTQ series of 4-bit quantization and compression models.
 
 ## Demo
 
 Full parameter fine-tuning of the LLaMA-3 8B model using a single GTX 3090 GPU with 24GB of graphics memory:
 
 <img src="assets/demo_llama3_8B_fpft.gif" width="960">
 
@@ -137,18 +154,24 @@
 ### Full-parameter fine-tuning
 
 Run the script as follows to fine-tune the quantized weights of the model on the target dataset. 
 The '--tune-qweight-only' parameter determines whether to fine-tune only the quantized weights or all weights, including non-quantized ones.
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python -m green_bit_llm.sft.finetune --model GreenBitAI/Qwen-1.5-1.8B-layer-mix-bpw-3.0 --dataset tatsu-lab/alpaca --optimizer DiodeMix --tune-qweight-only
+
+# AutoGPTQ model Q-SFT
+CUDA_VISIBLE_DEVICES=0 python -m green_bit_llm.sft.finetune --model astronomer/Llama-3-8B-Instruct-GPTQ-4-Bit --dataset tatsu-lab/alpaca --tune-qweight-only --batch-size 1
 ```
 
 ### Parameter efficient fine-tuning
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python -m green_bit_llm.sft.peft_lora --model GreenBitAI/Qwen-1.5-1.8B-layer-mix-bpw-3.0 --dataset tatsu-lab/alpaca --lr-fp 1e-6
+
+# AutoGPTQ model with Lora
+CUDA_VISIBLE_DEVICES=0 python -m green_bit_llm.sft.peft_lora --model astronomer/Llama-3-8B-Instruct-GPTQ-4-Bit --dataset tatsu-lab/alpaca --lr-fp 1e-6
 ```
 
 ## License
 We release our codes under the [Apache 2.0 License](LICENSE).
 Additionally, three packages are also partly based on third-party open-source codes. For detailed information, please refer to the description pages of the sub-projects.
```

### Comparing `green-bit-llm-0.1.0/green_bit_llm.egg-info/SOURCES.txt` & `green-bit-llm-0.2.0/green_bit_llm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 green_bit_llm/inference/chat_cli.py
 green_bit_llm/inference/conversation.py
 green_bit_llm/inference/sim_gen.py
 green_bit_llm/inference/utils.py
 green_bit_llm/sft/__init__.py
 green_bit_llm/sft/finetune.py
 green_bit_llm/sft/peft_lora.py
+green_bit_llm/sft/trainer.py
 green_bit_llm/sft/utils.py
 green_bit_llm/sft/optim/__init__.py
 green_bit_llm/sft/optim/adamw8bit.py
 green_bit_llm/sft/optim/bnb_optimizer.py
 green_bit_llm/sft/peft_utils/__init__.py
 green_bit_llm/sft/peft_utils/gba_lora.py
 green_bit_llm/sft/peft_utils/model.py
```

### Comparing `green-bit-llm-0.1.0/setup.py` & `green-bit-llm-0.2.0/setup.py`

 * *Files identical despite different names*

