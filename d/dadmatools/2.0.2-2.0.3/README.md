# Comparing `tmp/dadmatools-2.0.2.tar.gz` & `tmp/dadmatools-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dadmatools-2.0.2.tar", last modified: Fri Apr  5 11:39:16 2024, max compression
+gzip compressed data, was "dadmatools-2.0.3.tar", last modified: Wed May 22 11:45:54 2024, max compression
```

## Comparing `dadmatools-2.0.2.tar` & `dadmatools-2.0.3.tar`

### file list

```diff
@@ -1,308 +1,308 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.312985 dadmatools-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 11:39:10.000000 dadmatools-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22067 2024-04-05 11:39:16.312985 dadmatools-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20649 2024-04-05 11:39:10.000000 dadmatools-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.268985 dadmatools-2.0.2/dadmatools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.268985 dadmatools-2.0.2/dadmatools/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/dataset_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.268985 dadmatools-2.0.2/dadmatools/datasets/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.272985 dadmatools-2.0.2/dadmatools/datasets/datasets/Arman/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/Arman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/Arman/arman.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/Arman/info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.272985 dadmatools-2.0.2/dadmatools/datasets/datasets/FaSpell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/FaSpell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/FaSpell/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/FaSpell/sp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.272985 dadmatools-2.0.2/dadmatools/datasets/datasets/FarsTail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/FarsTail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/FarsTail/farstail.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/FarsTail/info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.272985 dadmatools-2.0.2/dadmatools/datasets/datasets/PersianNer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/PersianNer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/PersianNer/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/PersianNer/persian_ner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.272985 dadmatools-2.0.2/dadmatools/datasets/datasets/PersianTweets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/PersianTweets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/PersianTweets/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/PersianTweets/persian_tweets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.272985 dadmatools-2.0.2/dadmatools/datasets/datasets/Peyma/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/Peyma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/Peyma/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/Peyma/peyma.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.272985 dadmatools-2.0.2/dadmatools/datasets/datasets/TEP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/TEP/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/TEP/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/TEP/tep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.272985 dadmatools-2.0.2/dadmatools/datasets/datasets/Wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/Wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/Wikipedia/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/Wikipedia/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.272985 dadmatools-2.0.2/dadmatools/datasets/datasets/persent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/persent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/persent/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/persent/persent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.276985 dadmatools-2.0.2/dadmatools/datasets/datasets/persianNews/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/persianNews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/persianNews/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/persianNews/persian_news.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.276985 dadmatools-2.0.2/dadmatools/datasets/datasets/perudt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/perudt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/perudt/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/perudt/perudt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.276985 dadmatools-2.0.2/dadmatools/datasets/datasets/pnSummary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/pnSummary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/pnSummary/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/pnSummary/pn_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.276985 dadmatools-2.0.2/dadmatools/datasets/datasets/snappfoodSentiment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/snappfoodSentiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/snappfoodSentiment/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets/snappfoodSentiment/snappfood_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/datasets/datasets_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.276985 dadmatools-2.0.2/dadmatools/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/embeddings/available_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/embeddings/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/embeddings/embedding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/normalizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.276985 dadmatools-2.0.2/dadmatools/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15412 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.300985 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)    19872 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)    37406 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/adapter_bert.py
--rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/adapter_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    44978 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/adapter_model_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/adapter_modeling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/adapter_training.py
--rw-r--r--   0 runner    (1001) docker     (127)    17424 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/adapter_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.300985 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/benchmark/benchmark_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/benchmark/benchmark_args_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    28412 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/benchmark/benchmark_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.304985 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/serving.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/transformers_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_albert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_bart.py
--rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_bert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_camembert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_ctrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_distilbert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_electra.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_flaubert.py
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_longformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_marian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_mmbt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    13632 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_reformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_roberta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_t5.py
--rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_transfo_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_xlm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_xlm_roberta.py
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_xlnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_albert_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_bart_original_pytorch_checkpoint_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_bert_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_bert_pytorch_checkpoint_to_original_tf.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_dialogpt_original_pytorch_checkpoint_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_electra_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_gpt2_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_graph_to_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_longformer_original_pytorch_lightning_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    21395 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_marian_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_openai_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    14879 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_pytorch_checkpoint_to_tf2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_reformer_trax_checkpoint_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_roberta_original_pytorch_checkpoint_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_t5_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_transfo_xl_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_xlm_original_pytorch_checkpoint_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_xlnet_original_tf_checkpoint_to_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.304985 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/data_collator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.304985 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/datasets/glue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/datasets/language_modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.304985 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29765 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/metrics/squad_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.304985 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/processors/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22106 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/processors/glue.py
--rw-r--r--   0 runner    (1001) docker     (127)    29888 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/processors/squad.py
--rw-r--r--   0 runner    (1001) docker     (127)    14193 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/processors/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/processors/xnli.py
--rw-r--r--   0 runner    (1001) docker     (127)    18531 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/hf_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/hf_argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modelcard.py
--rw-r--r--   0 runner    (1001) docker     (127)    51030 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_albert.py
--rw-r--r--   0 runner    (1001) docker     (127)    80520 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)    50114 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_bart.py
--rw-r--r--   0 runner    (1001) docker     (127)    74134 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_bert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_camembert.py
--rw-r--r--   0 runner    (1001) docker     (127)    25021 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_ctrl.py
--rw-r--r--   0 runner    (1001) docker     (127)    39129 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_distilbert.py
--rw-r--r--   0 runner    (1001) docker     (127)    33492 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_electra.py
--rw-r--r--   0 runner    (1001) docker     (127)    18063 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16477 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_flaubert.py
--rw-r--r--   0 runner    (1001) docker     (127)    35380 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (127)    63557 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_longformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_marian.py
--rw-r--r--   0 runner    (1001) docker     (127)    18703 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_mmbt.py
--rw-r--r--   0 runner    (1001) docker     (127)    32330 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    76625 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_reformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    35015 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_roberta.py
--rw-r--r--   0 runner    (1001) docker     (127)    55030 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_t5.py
--rw-r--r--   0 runner    (1001) docker     (127)    52084 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_albert.py
--rw-r--r--   0 runner    (1001) docker     (127)    78625 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)    56704 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_bert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_camembert.py
--rw-r--r--   0 runner    (1001) docker     (127)    27829 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_ctrl.py
--rw-r--r--   0 runner    (1001) docker     (127)    39638 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_distilbert.py
--rw-r--r--   0 runner    (1001) docker     (127)    28838 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_electra.py
--rw-r--r--   0 runner    (1001) docker     (127)    15952 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_flaubert.py
--rw-r--r--   0 runner    (1001) docker     (127)    34917 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (127)    31257 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25458 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_roberta.py
--rw-r--r--   0 runner    (1001) docker     (127)    54221 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_t5.py
--rw-r--r--   0 runner    (1001) docker     (127)    36543 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_transfo_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_transfo_xl_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    86054 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39614 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_xlm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_xlm_roberta.py
--rw-r--r--   0 runner    (1001) docker     (127)    61710 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_xlnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40842 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_transfo_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_transfo_xl_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)   111279 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    52002 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_xlm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_xlm_roberta.py
--rw-r--r--   0 runner    (1001) docker     (127)    81566 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_xlnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/optimization_tf.py
--rw-r--r--   0 runner    (1001) docker     (127)    81433 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)    14507 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_albert.py
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_bart.py
--rw-r--r--   0 runner    (1001) docker     (127)    31317 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_bert.py
--rw-r--r--   0 runner    (1001) docker     (127)    10318 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_bert_japanese.py
--rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_camembert.py
--rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_ctrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_distilbert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_electra.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_flaubert.py
--rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_longformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_marian.py
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_reformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_roberta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8554 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_t5.py
--rw-r--r--   0 runner    (1001) docker     (127)    29179 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_transfo_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)   136046 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    36448 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_xlm.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_xlm_roberta.py
--rw-r--r--   0 runner    (1001) docker     (127)    14253 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_xlnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17848 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/trainer_tf.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/trainer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/training_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/training_args_tf.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.304985 dadmatools-2.0.2/dadmatools/pipeline/informal2formal/
--rw-r--r--   0 runner    (1001) docker     (127)    30380 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/informal2formal/OneShotTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20032 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/informal2formal/VerbHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/informal2formal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/informal2formal/download_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/informal2formal/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/informal2formal/formality_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/informal2formal/kenlm_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/informal2formal/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/informal2formal/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11215 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/informal2formal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.308985 dadmatools-2.0.2/dadmatools/pipeline/iterators/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/iterators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/iterators/lemmatizer_iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/iterators/mwt_iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/iterators/ner_iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10318 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/iterators/sent_iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)    19410 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/iterators/tagger_iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/iterators/tokenizer_iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)    61418 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/language.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.308985 dadmatools-2.0.2/dadmatools/pipeline/layers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/layers/crf_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23270 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/layers/seq2seq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.308985 dadmatools-2.0.2/dadmatools/pipeline/models/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/models/base_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    15301 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/models/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)    21659 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/models/lemma_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/models/mwt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    25415 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/models/spellchecker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.308985 dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    37698 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20838 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/vocab.py
--rw-r--r--   0 runner    (1001) docker     (127)    37677 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/tpipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.312985 dadmatools-2.0.2/dadmatools/pipeline/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14220 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/base_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/chuliu_edmonds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/conll.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.312985 dadmatools-2.0.2/dadmatools/pipeline/utils/mwt_lemma_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/mwt_lemma_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/mwt_lemma_utils/mwt_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12588 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/mwt_lemma_utils/seq2seq_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/mwt_lemma_utils/seq2seq_vocabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/ner_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/posdep_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.312985 dadmatools-2.0.2/dadmatools/pipeline/utils/scorers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/scorers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28665 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/scorers/conll18_ud_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/scorers/ner_scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/scorers/sent_scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/sent_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/tbinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    13620 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/pipeline/utils/tokenizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.312985 dadmatools-2.0.2/dadmatools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/utils/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)    27448 2024-04-05 11:39:10.000000 dadmatools-2.0.2/dadmatools/utils/stopwords-fa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:39:16.312985 dadmatools-2.0.2/dadmatools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22067 2024-04-05 11:39:16.000000 dadmatools-2.0.2/dadmatools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15272 2024-04-05 11:39:16.000000 dadmatools-2.0.2/dadmatools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 11:39:16.000000 dadmatools-2.0.2/dadmatools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-05 11:39:16.000000 dadmatools-2.0.2/dadmatools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 11:39:16.000000 dadmatools-2.0.2/dadmatools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 11:39:16.312985 dadmatools-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-05 11:39:10.000000 dadmatools-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.576228 dadmatools-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 11:45:50.000000 dadmatools-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22096 2024-05-22 11:45:54.576228 dadmatools-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20649 2024-05-22 11:45:50.000000 dadmatools-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.524228 dadmatools-2.0.3/dadmatools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.528228 dadmatools-2.0.3/dadmatools/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/dataset_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.528228 dadmatools-2.0.3/dadmatools/datasets/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.528228 dadmatools-2.0.3/dadmatools/datasets/datasets/Arman/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/Arman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/Arman/arman.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/Arman/info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.528228 dadmatools-2.0.3/dadmatools/datasets/datasets/FaSpell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/FaSpell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/FaSpell/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/FaSpell/sp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.528228 dadmatools-2.0.3/dadmatools/datasets/datasets/FarsTail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/FarsTail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/FarsTail/farstail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/FarsTail/info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.528228 dadmatools-2.0.3/dadmatools/datasets/datasets/PersianNer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/PersianNer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/PersianNer/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/PersianNer/persian_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.528228 dadmatools-2.0.3/dadmatools/datasets/datasets/PersianTweets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/PersianTweets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/PersianTweets/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/PersianTweets/persian_tweets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.532228 dadmatools-2.0.3/dadmatools/datasets/datasets/Peyma/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/Peyma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/Peyma/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/Peyma/peyma.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.532228 dadmatools-2.0.3/dadmatools/datasets/datasets/TEP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/TEP/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/TEP/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/TEP/tep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.532228 dadmatools-2.0.3/dadmatools/datasets/datasets/Wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/Wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/Wikipedia/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/Wikipedia/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.532228 dadmatools-2.0.3/dadmatools/datasets/datasets/persent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/persent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/persent/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/persent/persent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.532228 dadmatools-2.0.3/dadmatools/datasets/datasets/persianNews/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/persianNews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/persianNews/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/persianNews/persian_news.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.532228 dadmatools-2.0.3/dadmatools/datasets/datasets/perudt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/perudt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/perudt/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/perudt/perudt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.532228 dadmatools-2.0.3/dadmatools/datasets/datasets/pnSummary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/pnSummary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/pnSummary/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/pnSummary/pn_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.536228 dadmatools-2.0.3/dadmatools/datasets/datasets/snappfoodSentiment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/snappfoodSentiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/snappfoodSentiment/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets/snappfoodSentiment/snappfood_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/datasets/datasets_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.536228 dadmatools-2.0.3/dadmatools/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/embeddings/available_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/embeddings/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/embeddings/embedding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/normalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.536228 dadmatools-2.0.3/dadmatools/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15412 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.560228 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)    19872 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37406 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/adapter_bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/adapter_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44978 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/adapter_model_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/adapter_modeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/adapter_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17424 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/adapter_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.564228 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/benchmark/benchmark_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/benchmark/benchmark_args_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28412 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/benchmark/benchmark_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.564228 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/serving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/transformers_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_albert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_bart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_camembert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_distilbert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_electra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_flaubert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_longformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_marian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_mmbt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13632 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_reformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_roberta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_transfo_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_xlm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_xlm_roberta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_xlnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_albert_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_bart_original_pytorch_checkpoint_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_bert_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_bert_pytorch_checkpoint_to_original_tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_dialogpt_original_pytorch_checkpoint_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_electra_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_gpt2_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_graph_to_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_longformer_original_pytorch_lightning_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21395 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_marian_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_openai_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14879 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_pytorch_checkpoint_to_tf2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_reformer_trax_checkpoint_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_roberta_original_pytorch_checkpoint_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_t5_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_transfo_xl_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_xlm_original_pytorch_checkpoint_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_xlnet_original_tf_checkpoint_to_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.564228 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/data_collator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.564228 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/datasets/glue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/datasets/language_modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.564228 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29765 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/metrics/squad_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.568229 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22106 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/processors/glue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29888 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/processors/squad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14193 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/processors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/processors/xnli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18531 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/hf_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/hf_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modelcard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51030 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_albert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80520 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50114 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_bart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74134 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_camembert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25021 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39129 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_distilbert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33492 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_electra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18063 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16477 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_flaubert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35380 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63557 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_longformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_marian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18703 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_mmbt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32330 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76625 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_reformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35015 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_roberta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55030 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52084 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_albert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78625 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56704 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_camembert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27829 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39638 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_distilbert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28838 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_electra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15952 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_flaubert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34917 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31257 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25458 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_roberta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54221 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36543 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_transfo_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_transfo_xl_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86054 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39614 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_xlm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_xlm_roberta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61710 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_xlnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40842 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_transfo_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_transfo_xl_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111279 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52002 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_xlm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_xlm_roberta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81566 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_xlnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/optimization_tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81433 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14507 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_albert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_bart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31317 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10318 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_bert_japanese.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_camembert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_distilbert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_electra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_flaubert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_longformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_marian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_reformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_roberta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8554 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29179 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_transfo_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136046 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36448 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_xlm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_xlm_roberta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14253 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_xlnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17848 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/trainer_tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/trainer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/training_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/training_args_tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.568229 dadmatools-2.0.3/dadmatools/pipeline/informal2formal/
+-rw-r--r--   0 runner    (1001) docker     (127)    30380 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/informal2formal/OneShotTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20032 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/informal2formal/VerbHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/informal2formal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/informal2formal/download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/informal2formal/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/informal2formal/formality_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/informal2formal/kenlm_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/informal2formal/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/informal2formal/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11215 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/informal2formal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.568229 dadmatools-2.0.3/dadmatools/pipeline/iterators/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/iterators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/iterators/lemmatizer_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/iterators/mwt_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/iterators/ner_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10318 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/iterators/sent_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19410 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/iterators/tagger_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/iterators/tokenizer_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61418 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/language.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.568229 dadmatools-2.0.3/dadmatools/pipeline/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/layers/crf_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23270 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/layers/seq2seq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.572229 dadmatools-2.0.3/dadmatools/pipeline/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/models/base_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15301 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/models/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21659 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/models/lemma_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/models/mwt_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25415 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/models/spellchecker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.572229 dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37698 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20838 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/vocab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37677 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/tpipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.572229 dadmatools-2.0.3/dadmatools/pipeline/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14220 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/chuliu_edmonds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/conll.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.572229 dadmatools-2.0.3/dadmatools/pipeline/utils/mwt_lemma_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/mwt_lemma_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/mwt_lemma_utils/mwt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12588 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/mwt_lemma_utils/seq2seq_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/mwt_lemma_utils/seq2seq_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/ner_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/posdep_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.576228 dadmatools-2.0.3/dadmatools/pipeline/utils/scorers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/scorers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28665 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/scorers/conll18_ud_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/scorers/ner_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/scorers/sent_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/sent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/tbinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13620 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/pipeline/utils/tokenizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.576228 dadmatools-2.0.3/dadmatools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/utils/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27448 2024-05-22 11:45:50.000000 dadmatools-2.0.3/dadmatools/utils/stopwords-fa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:45:54.576228 dadmatools-2.0.3/dadmatools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22096 2024-05-22 11:45:54.000000 dadmatools-2.0.3/dadmatools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15272 2024-05-22 11:45:54.000000 dadmatools-2.0.3/dadmatools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 11:45:54.000000 dadmatools-2.0.3/dadmatools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-22 11:45:54.000000 dadmatools-2.0.3/dadmatools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 11:45:54.000000 dadmatools-2.0.3/dadmatools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 11:45:54.576228 dadmatools-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-22 11:45:50.000000 dadmatools-2.0.3/setup.py
```

### Comparing `dadmatools-2.0.2/LICENSE` & `dadmatools-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/PKG-INFO` & `dadmatools-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dadmatools
-Version: 2.0.2
+Version: 2.0.3
 Summary: DadmaTools is a Persian NLP toolkit
 Home-page: https://github.com/Dadmatech/DadmaTools
 Author: Dadmatech AI Company
 Author-email: info@dadmatech.ir
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License 
 Classifier: Operating System :: OS Independent
@@ -40,14 +40,15 @@
 Requires-Dist: tokenizers>=0.7.0
 Requires-Dist: regex!=2019.12.17
 Requires-Dist: packaging
 Requires-Dist: sentencepiece
 Requires-Dist: sacremoses
 Requires-Dist: fasttext
 Requires-Dist: kenlm
+Requires-Dist: emoji==2.10.0
 
 <!-- <h1 align="center">
   <img src="images/dadmatech.jpeg"  width="150"  />
    Dadmatools
 </h1> -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dadmatools Version: 2.0.2 Summary: DadmaTools is a
+Metadata-Version: 2.1 Name: dadmatools Version: 2.0.3 Summary: DadmaTools is a
 Persian NLP toolkit Home-page: https://github.com/Dadmatech/DadmaTools Author:
 Dadmatech AI Company Author-email: info@dadmatech.ir Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: bpemb>=0.3.3 Requires-
 Dist: nltk Requires-Dist: folium>=0.2.1 Requires-Dist: spacy>=3.0.0 Requires-
 Dist: torch>=1.7.1 Requires-Dist: transformers>=4.9.1 Requires-Dist:
@@ -12,15 +12,15 @@
 supar==1.1.2 Requires-Dist: gensim>=3.6.0 Requires-Dist: conllu Requires-Dist:
 gdown>=4.3.1 Requires-Dist: py7zr>=0.17.2 Requires-Dist: html2text Requires-
 Dist: tf-estimator-nightly==2.8.0.dev2021122109 Requires-Dist: scikit-
 learn>=0.24.2 Requires-Dist: numpy Requires-Dist: protobuf Requires-Dist:
 requests Requires-Dist: tqdm>=4.27 Requires-Dist: langid==1.1.6 Requires-Dist:
 filelock Requires-Dist: tokenizers>=0.7.0 Requires-Dist: regex!=2019.12.17
 Requires-Dist: packaging Requires-Dist: sentencepiece Requires-Dist: sacremoses
-Requires-Dist: fasttext Requires-Dist: kenlm
+Requires-Dist: fasttext Requires-Dist: kenlm Requires-Dist: emoji==2.10.0
            ********** DDaaddmmaaTToooollss:: AA PPyytthhoonn NNLLPP LLiibbrraarryy ffoorr PPeerrssiiaann **********
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_d_a_d_m_a_t_o_o_l_s_._s_v_g_][https://img.shields.io/badge/
               license-Apache%202-blue.svg]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]
   **** NNaammeedd EEnnttiittyy RReeccooggnniittiioonn || PPaarrtt ooff SSppeeeecchh TTaaggggiinngg || DDeeppeennddeennccyy PPaarrssiinngg ||
                              IInnffoorrmmaall TToo FFoorrmmaall ****
         **** CCoonnssttiittuueennccyy PPaarrssiinngg || CChhuunnkkiinngg || KKaassrreehh EEzzaaffee DDeetteeccttiioonn ****
  **** SSppeellllcchheecckkeerr || NNoorrmmaalliizzeerr || TTookkeenniizzeerr || LLeemmmmaattiizzeerr || SSeennttiimmeenntt AAnnaallyyssiiss ****
```

### Comparing `dadmatools-2.0.2/README.md` & `dadmatools-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/__init__.py` & `dadmatools-2.0.3/dadmatools/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/base.py` & `dadmatools-2.0.3/dadmatools/datasets/base.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/dataset_utils.py` & `dadmatools-2.0.3/dadmatools/datasets/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/datasets/Arman/arman.py` & `dadmatools-2.0.3/dadmatools/datasets/datasets/Arman/arman.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/datasets/FaSpell/sp.py` & `dadmatools-2.0.3/dadmatools/datasets/datasets/FaSpell/sp.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/datasets/FarsTail/farstail.py` & `dadmatools-2.0.3/dadmatools/datasets/datasets/FarsTail/farstail.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/datasets/PersianNer/persian_ner.py` & `dadmatools-2.0.3/dadmatools/datasets/datasets/PersianNer/persian_ner.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/datasets/PersianTweets/persian_tweets.py` & `dadmatools-2.0.3/dadmatools/datasets/datasets/PersianTweets/persian_tweets.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/datasets/Peyma/peyma.py` & `dadmatools-2.0.3/dadmatools/datasets/datasets/Peyma/peyma.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/datasets/TEP/tep.py` & `dadmatools-2.0.3/dadmatools/datasets/datasets/TEP/tep.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/datasets/Wikipedia/wikipedia.py` & `dadmatools-2.0.3/dadmatools/datasets/datasets/Wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/datasets/persent/persent.py` & `dadmatools-2.0.3/dadmatools/datasets/datasets/persent/persent.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/datasets/persianNews/persian_news.py` & `dadmatools-2.0.3/dadmatools/datasets/datasets/persianNews/persian_news.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/datasets/perudt/perudt.py` & `dadmatools-2.0.3/dadmatools/datasets/datasets/perudt/perudt.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/datasets/pnSummary/pn_summary.py` & `dadmatools-2.0.3/dadmatools/datasets/datasets/pnSummary/pn_summary.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/datasets/snappfoodSentiment/snappfood_sentiment.py` & `dadmatools-2.0.3/dadmatools/datasets/datasets/snappfoodSentiment/snappfood_sentiment.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/datasets/datasets_info.py` & `dadmatools-2.0.3/dadmatools/datasets/datasets_info.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/embeddings/available_models.py` & `dadmatools-2.0.3/dadmatools/embeddings/available_models.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/embeddings/embedding.py` & `dadmatools-2.0.3/dadmatools/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/embeddings/embedding_utils.py` & `dadmatools-2.0.3/dadmatools/embeddings/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/normalizer.py` & `dadmatools-2.0.3/dadmatools/normalizer.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/__init__.py` & `dadmatools-2.0.3/dadmatools/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/__main__.py` & `dadmatools-2.0.3/dadmatools/pipeline/__main__.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/__init__.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/activations.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/activations.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/adapter_bert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/adapter_bert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/adapter_config.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/adapter_config.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/adapter_model_mixin.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/adapter_model_mixin.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/adapter_modeling.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/adapter_modeling.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/adapter_training.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/adapter_training.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/adapter_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/adapter_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/benchmark/benchmark.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/benchmark/benchmark_args.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/benchmark/benchmark_args.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/benchmark/benchmark_args_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/benchmark/benchmark_args_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/benchmark/benchmark_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/convert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/convert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/download.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/download.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/env.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/env.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/run.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/run.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/serving.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/serving.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/train.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/train.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/transformers_cli.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/transformers_cli.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/commands/user.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/commands/user.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_albert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_albert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_auto.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_auto.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_bart.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_bart.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_bert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_bert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_camembert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_camembert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_ctrl.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_ctrl.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_distilbert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_distilbert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_electra.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_electra.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_encoder_decoder.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_flaubert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_flaubert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_gpt2.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_gpt2.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_longformer.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_longformer.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_marian.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_marian.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_mmbt.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_mmbt.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_openai.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_openai.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_reformer.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_reformer.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_roberta.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_roberta.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_t5.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_t5.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_transfo_xl.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_transfo_xl.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_xlm.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_xlm.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_xlm_roberta.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/configuration_xlnet.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/configuration_xlnet.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_albert_original_tf_checkpoint_to_pytorch.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_albert_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_bart_original_pytorch_checkpoint_to_pytorch.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_bart_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_bert_original_tf_checkpoint_to_pytorch.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_bert_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_bert_pytorch_checkpoint_to_original_tf.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_bert_pytorch_checkpoint_to_original_tf.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_dialogpt_original_pytorch_checkpoint_to_pytorch.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_dialogpt_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_electra_original_tf_checkpoint_to_pytorch.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_electra_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_gpt2_original_tf_checkpoint_to_pytorch.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_gpt2_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_graph_to_onnx.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_graph_to_onnx.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_longformer_original_pytorch_lightning_to_pytorch.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_longformer_original_pytorch_lightning_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_marian_to_pytorch.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_marian_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_openai_original_tf_checkpoint_to_pytorch.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_openai_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_pytorch_checkpoint_to_tf2.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_pytorch_checkpoint_to_tf2.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_reformer_trax_checkpoint_to_pytorch.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_reformer_trax_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_roberta_original_pytorch_checkpoint_to_pytorch.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_roberta_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_t5_original_tf_checkpoint_to_pytorch.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_t5_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_transfo_xl_original_tf_checkpoint_to_pytorch.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_transfo_xl_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_xlm_original_pytorch_checkpoint_to_pytorch.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_xlm_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/convert_xlnet_original_tf_checkpoint_to_pytorch.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/convert_xlnet_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/__init__.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/__init__.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/data_collator.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/data_collator.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/datasets/glue.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/datasets/glue.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/datasets/language_modeling.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/datasets/language_modeling.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/metrics/__init__.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/metrics/squad_metrics.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/metrics/squad_metrics.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/processors/__init__.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/processors/glue.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/processors/glue.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/processors/squad.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/processors/squad.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/processors/utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/processors/utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/data/processors/xnli.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/data/processors/xnli.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/file_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/file_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/hf_api.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/hf_api.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/hf_argparser.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/hf_argparser.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modelcard.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modelcard.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_albert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_albert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_auto.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_auto.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_bart.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_bart.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_bert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_bert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_camembert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_camembert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_ctrl.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_ctrl.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_distilbert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_distilbert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_electra.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_electra.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_encoder_decoder.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_flaubert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_flaubert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_gpt2.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_gpt2.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_longformer.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_longformer.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_marian.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_marian.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_mmbt.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_mmbt.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_openai.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_openai.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_reformer.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_reformer.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_roberta.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_roberta.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_t5.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_t5.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_albert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_albert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_auto.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_auto.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_bert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_bert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_camembert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_camembert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_ctrl.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_ctrl.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_distilbert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_distilbert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_electra.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_electra.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_flaubert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_flaubert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_gpt2.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_gpt2.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_openai.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_openai.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_pytorch_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_roberta.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_roberta.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_t5.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_t5.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_transfo_xl.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_transfo_xl.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_transfo_xl_utilities.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_transfo_xl_utilities.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_xlm.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_xlm.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_xlm_roberta.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_tf_xlnet.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_tf_xlnet.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_transfo_xl.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_transfo_xl.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_transfo_xl_utilities.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_transfo_xl_utilities.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_xlm.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_xlm.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_xlm_roberta.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/modeling_xlnet.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/modeling_xlnet.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/optimization.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/optimization.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/optimization_tf.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/optimization_tf.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/pipelines.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/pipelines.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_albert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_albert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_auto.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_auto.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_bart.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_bart.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_bert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_bert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_bert_japanese.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_bert_japanese.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_camembert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_camembert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_ctrl.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_ctrl.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_distilbert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_distilbert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_electra.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_electra.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_flaubert.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_flaubert.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_gpt2.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_gpt2.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_longformer.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_longformer.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_marian.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_marian.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_openai.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_openai.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_reformer.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_reformer.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_roberta.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_roberta.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_t5.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_t5.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_transfo_xl.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_transfo_xl.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_xlm.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_xlm.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_xlm_roberta.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/tokenization_xlnet.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/tokenization_xlnet.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/trainer.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/trainer.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/trainer_tf.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/trainer_tf.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/trainer_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/training_args.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/training_args.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/adapter_transformers/training_args_tf.py` & `dadmatools-2.0.3/dadmatools/pipeline/adapter_transformers/training_args_tf.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/config.py` & `dadmatools-2.0.3/dadmatools/pipeline/config.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/informal2formal/OneShotTransformer.py` & `dadmatools-2.0.3/dadmatools/pipeline/informal2formal/OneShotTransformer.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/informal2formal/VerbHandler.py` & `dadmatools-2.0.3/dadmatools/pipeline/informal2formal/VerbHandler.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/informal2formal/download_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/informal2formal/download_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/informal2formal/formality_transformer.py` & `dadmatools-2.0.3/dadmatools/pipeline/informal2formal/formality_transformer.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/informal2formal/kenlm_wrapper.py` & `dadmatools-2.0.3/dadmatools/pipeline/informal2formal/kenlm_wrapper.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/informal2formal/main.py` & `dadmatools-2.0.3/dadmatools/pipeline/informal2formal/main.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/informal2formal/tokenizer.py` & `dadmatools-2.0.3/dadmatools/pipeline/informal2formal/tokenizer.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/informal2formal/utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/informal2formal/utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/iterators/lemmatizer_iterators.py` & `dadmatools-2.0.3/dadmatools/pipeline/iterators/lemmatizer_iterators.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/iterators/mwt_iterators.py` & `dadmatools-2.0.3/dadmatools/pipeline/iterators/mwt_iterators.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/iterators/ner_iterators.py` & `dadmatools-2.0.3/dadmatools/pipeline/iterators/ner_iterators.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/iterators/sent_iterators.py` & `dadmatools-2.0.3/dadmatools/pipeline/iterators/sent_iterators.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/iterators/tagger_iterators.py` & `dadmatools-2.0.3/dadmatools/pipeline/iterators/tagger_iterators.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/iterators/tokenizer_iterators.py` & `dadmatools-2.0.3/dadmatools/pipeline/iterators/tokenizer_iterators.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/language.py` & `dadmatools-2.0.3/dadmatools/pipeline/language.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/layers/crf_layer.py` & `dadmatools-2.0.3/dadmatools/pipeline/layers/crf_layer.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/layers/seq2seq.py` & `dadmatools-2.0.3/dadmatools/pipeline/layers/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/models/base_models.py` & `dadmatools-2.0.3/dadmatools/pipeline/models/base_models.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/models/classifiers.py` & `dadmatools-2.0.3/dadmatools/pipeline/models/classifiers.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/models/lemma_model.py` & `dadmatools-2.0.3/dadmatools/pipeline/models/lemma_model.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/models/mwt_model.py` & `dadmatools-2.0.3/dadmatools/pipeline/models/mwt_model.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/models/spellchecker.py` & `dadmatools-2.0.3/dadmatools/pipeline/models/spellchecker.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/data.py` & `dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/data.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/doc.py` & `dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/doc.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/download.py` & `dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/download.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/model.py` & `dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/model.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/tokenizer.py` & `dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/tokenizer.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/trainer.py` & `dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/trainer.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/persian_tokenization/vocab.py` & `dadmatools-2.0.3/dadmatools/pipeline/persian_tokenization/vocab.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/tpipeline.py` & `dadmatools-2.0.3/dadmatools/pipeline/tpipeline.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/utils/base_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/utils/base_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/utils/chuliu_edmonds.py` & `dadmatools-2.0.3/dadmatools/pipeline/utils/chuliu_edmonds.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/utils/conll.py` & `dadmatools-2.0.3/dadmatools/pipeline/utils/conll.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/utils/mwt_lemma_utils/mwt_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/utils/mwt_lemma_utils/mwt_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/utils/mwt_lemma_utils/seq2seq_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/utils/mwt_lemma_utils/seq2seq_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/utils/mwt_lemma_utils/seq2seq_vocabs.py` & `dadmatools-2.0.3/dadmatools/pipeline/utils/mwt_lemma_utils/seq2seq_vocabs.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/utils/ner_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/utils/ner_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/utils/posdep_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/utils/posdep_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/utils/scorers/conll18_ud_eval.py` & `dadmatools-2.0.3/dadmatools/pipeline/utils/scorers/conll18_ud_eval.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/utils/scorers/ner_scorer.py` & `dadmatools-2.0.3/dadmatools/pipeline/utils/scorers/ner_scorer.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/utils/sent_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/utils/sent_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/utils/tbinfo.py` & `dadmatools-2.0.3/dadmatools/pipeline/utils/tbinfo.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/pipeline/utils/tokenizer_utils.py` & `dadmatools-2.0.3/dadmatools/pipeline/utils/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/utils/patterns.py` & `dadmatools-2.0.3/dadmatools/utils/patterns.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools/utils/stopwords-fa.py` & `dadmatools-2.0.3/dadmatools/utils/stopwords-fa.py`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/dadmatools.egg-info/PKG-INFO` & `dadmatools-2.0.3/dadmatools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dadmatools
-Version: 2.0.2
+Version: 2.0.3
 Summary: DadmaTools is a Persian NLP toolkit
 Home-page: https://github.com/Dadmatech/DadmaTools
 Author: Dadmatech AI Company
 Author-email: info@dadmatech.ir
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License 
 Classifier: Operating System :: OS Independent
@@ -40,14 +40,15 @@
 Requires-Dist: tokenizers>=0.7.0
 Requires-Dist: regex!=2019.12.17
 Requires-Dist: packaging
 Requires-Dist: sentencepiece
 Requires-Dist: sacremoses
 Requires-Dist: fasttext
 Requires-Dist: kenlm
+Requires-Dist: emoji==2.10.0
 
 <!-- <h1 align="center">
   <img src="images/dadmatech.jpeg"  width="150"  />
    Dadmatools
 </h1> -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dadmatools Version: 2.0.2 Summary: DadmaTools is a
+Metadata-Version: 2.1 Name: dadmatools Version: 2.0.3 Summary: DadmaTools is a
 Persian NLP toolkit Home-page: https://github.com/Dadmatech/DadmaTools Author:
 Dadmatech AI Company Author-email: info@dadmatech.ir Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: bpemb>=0.3.3 Requires-
 Dist: nltk Requires-Dist: folium>=0.2.1 Requires-Dist: spacy>=3.0.0 Requires-
 Dist: torch>=1.7.1 Requires-Dist: transformers>=4.9.1 Requires-Dist:
@@ -12,15 +12,15 @@
 supar==1.1.2 Requires-Dist: gensim>=3.6.0 Requires-Dist: conllu Requires-Dist:
 gdown>=4.3.1 Requires-Dist: py7zr>=0.17.2 Requires-Dist: html2text Requires-
 Dist: tf-estimator-nightly==2.8.0.dev2021122109 Requires-Dist: scikit-
 learn>=0.24.2 Requires-Dist: numpy Requires-Dist: protobuf Requires-Dist:
 requests Requires-Dist: tqdm>=4.27 Requires-Dist: langid==1.1.6 Requires-Dist:
 filelock Requires-Dist: tokenizers>=0.7.0 Requires-Dist: regex!=2019.12.17
 Requires-Dist: packaging Requires-Dist: sentencepiece Requires-Dist: sacremoses
-Requires-Dist: fasttext Requires-Dist: kenlm
+Requires-Dist: fasttext Requires-Dist: kenlm Requires-Dist: emoji==2.10.0
            ********** DDaaddmmaaTToooollss:: AA PPyytthhoonn NNLLPP LLiibbrraarryy ffoorr PPeerrssiiaann **********
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_d_a_d_m_a_t_o_o_l_s_._s_v_g_][https://img.shields.io/badge/
               license-Apache%202-blue.svg]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]
   **** NNaammeedd EEnnttiittyy RReeccooggnniittiioonn || PPaarrtt ooff SSppeeeecchh TTaaggggiinngg || DDeeppeennddeennccyy PPaarrssiinngg ||
                              IInnffoorrmmaall TToo FFoorrmmaall ****
         **** CCoonnssttiittuueennccyy PPaarrssiinngg || CChhuunnkkiinngg || KKaassrreehh EEzzaaffee DDeetteeccttiioonn ****
  **** SSppeellllcchheecckkeerr || NNoorrmmaalliizzeerr || TTookkeenniizzeerr || LLeemmmmaattiizzeerr || SSeennttiimmeenntt AAnnaallyyssiiss ****
```

### Comparing `dadmatools-2.0.2/dadmatools.egg-info/SOURCES.txt` & `dadmatools-2.0.3/dadmatools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dadmatools-2.0.2/setup.py` & `dadmatools-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dadmatools",
-    version="2.0.2",
+    version="2.0.3",
     author="Dadmatech AI Company",
     author_email="info@dadmatech.ir",
     description="DadmaTools is a Persian NLP toolkit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Dadmatech/DadmaTools",
     packages=setuptools.find_packages(),
@@ -44,14 +44,15 @@
         'tokenizers>=0.7.0',
         'regex != 2019.12.17',
         'packaging',
         'sentencepiece',
         'sacremoses',
         'fasttext',
         'kenlm',
+        'emoji==2.10.0',
     ],
 
     dependency_links = [
         'git+https://github.com/kpu/kenlm@master#egg=kenlm',
     ],
 
     classifiers=[
```

