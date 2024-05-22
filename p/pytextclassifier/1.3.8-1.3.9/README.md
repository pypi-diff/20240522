# Comparing `tmp/pytextclassifier-1.3.8.tar.gz` & `tmp/pytextclassifier-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytextclassifier-1.3.8.tar", last modified: Thu May  9 02:21:46 2024, max compression
+gzip compressed data, was "pytextclassifier-1.3.9.tar", last modified: Wed May 22 03:33:52 2024, max compression
```

## Comparing `pytextclassifier-1.3.8.tar` & `pytextclassifier-1.3.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-05-09 02:21:46.043271 pytextclassifier-1.3.8/
--rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:50.000000 pytextclassifier-1.3.8/LICENSE
--rw-r--r--   0 xuming     (501) staff       (20)    22590 2024-05-09 02:21:46.043678 pytextclassifier-1.3.8/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    21802 2024-05-09 02:20:52.000000 pytextclassifier-1.3.8/README.md
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-05-09 02:21:46.041489 pytextclassifier-1.3.8/examples/
--rw-r--r--   0 xuming     (501) staff       (20)   616465 2022-03-29 07:45:47.000000 pytextclassifier-1.3.8/examples/thucnews_train_1w.txt
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-05-09 02:21:46.038761 pytextclassifier-1.3.8/pytextclassifier/
--rw-r--r--   0 xuming     (501) staff       (20)      640 2024-05-09 02:20:26.000000 pytextclassifier-1.3.8/pytextclassifier/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     2468 2023-06-14 12:38:54.000000 pytextclassifier-1.3.8/pytextclassifier/base_classifier.py
--rw-r--r--   0 xuming     (501) staff       (20)    39035 2023-06-14 12:38:54.000000 pytextclassifier-1.3.8/pytextclassifier/bert_classfication_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    87597 2024-05-09 02:10:56.000000 pytextclassifier-1.3.8/pytextclassifier/bert_classification_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    11338 2024-05-09 02:17:22.000000 pytextclassifier-1.3.8/pytextclassifier/bert_classifier.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    29987 2023-05-09 08:58:29.000000 pytextclassifier-1.3.8/pytextclassifier/bert_multi_label_classification_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    11050 2023-10-18 04:08:34.000000 pytextclassifier-1.3.8/pytextclassifier/classic_classifier.py
--rw-r--r--   0 xuming     (501) staff       (20)     1329 2023-10-18 04:08:34.000000 pytextclassifier-1.3.8/pytextclassifier/data_helper.py
--rw-r--r--   0 xuming     (501) staff       (20)    21704 2023-10-18 04:11:21.000000 pytextclassifier-1.3.8/pytextclassifier/fasttext_classifier.py
--rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 pytextclassifier-1.3.8/pytextclassifier/stopwords.txt
--rw-r--r--   0 xuming     (501) staff       (20)     7304 2023-05-09 08:44:44.000000 pytextclassifier-1.3.8/pytextclassifier/textcluster.py
--rw-r--r--   0 xuming     (501) staff       (20)    19072 2023-10-18 04:11:21.000000 pytextclassifier-1.3.8/pytextclassifier/textcnn_classifier.py
--rw-r--r--   0 xuming     (501) staff       (20)    19709 2023-10-18 04:11:21.000000 pytextclassifier-1.3.8/pytextclassifier/textrnn_classifier.py
--rw-r--r--   0 xuming     (501) staff       (20)      852 2022-04-12 06:51:36.000000 pytextclassifier-1.3.8/pytextclassifier/time_util.py
--rw-r--r--   0 xuming     (501) staff       (20)     2331 2023-06-14 12:38:54.000000 pytextclassifier-1.3.8/pytextclassifier/tokenizer.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-05-09 02:21:46.041074 pytextclassifier-1.3.8/pytextclassifier.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    22590 2024-05-09 02:21:45.000000 pytextclassifier-1.3.8/pytextclassifier.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)      848 2024-05-09 02:21:45.000000 pytextclassifier-1.3.8/pytextclassifier.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2024-05-09 02:21:45.000000 pytextclassifier-1.3.8/pytextclassifier.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)       52 2024-05-09 02:21:45.000000 pytextclassifier-1.3.8/pytextclassifier.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)       17 2024-05-09 02:21:45.000000 pytextclassifier-1.3.8/pytextclassifier.egg-info/top_level.txt
--rw-r--r--   0 xuming     (501) staff       (20)      309 2024-05-09 02:21:46.044943 pytextclassifier-1.3.8/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1444 2024-05-09 02:20:26.000000 pytextclassifier-1.3.8/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-05-22 03:33:52.918550 pytextclassifier-1.3.9/
+-rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:50.000000 pytextclassifier-1.3.9/LICENSE
+-rw-r--r--   0 xuming     (501) staff       (20)    22590 2024-05-22 03:33:52.918997 pytextclassifier-1.3.9/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    21802 2024-05-09 02:20:52.000000 pytextclassifier-1.3.9/README.md
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-05-22 03:33:52.913851 pytextclassifier-1.3.9/examples/
+-rw-r--r--   0 xuming     (501) staff       (20)   616465 2022-03-29 07:45:47.000000 pytextclassifier-1.3.9/examples/thucnews_train_1w.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-05-22 03:33:52.909817 pytextclassifier-1.3.9/pytextclassifier/
+-rw-r--r--   0 xuming     (501) staff       (20)      640 2024-05-22 03:31:13.000000 pytextclassifier-1.3.9/pytextclassifier/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2468 2023-06-14 12:38:54.000000 pytextclassifier-1.3.9/pytextclassifier/base_classifier.py
+-rw-r--r--   0 xuming     (501) staff       (20)    39035 2023-06-14 12:38:54.000000 pytextclassifier-1.3.9/pytextclassifier/bert_classfication_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    86241 2024-05-22 03:29:14.000000 pytextclassifier-1.3.9/pytextclassifier/bert_classification_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    11338 2024-05-09 02:17:22.000000 pytextclassifier-1.3.9/pytextclassifier/bert_classifier.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    14846 2024-05-22 03:26:09.000000 pytextclassifier-1.3.9/pytextclassifier/bert_multi_label_classification_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    11050 2023-10-18 04:08:34.000000 pytextclassifier-1.3.9/pytextclassifier/classic_classifier.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1329 2023-10-18 04:08:34.000000 pytextclassifier-1.3.9/pytextclassifier/data_helper.py
+-rw-r--r--   0 xuming     (501) staff       (20)    21704 2023-10-18 04:11:21.000000 pytextclassifier-1.3.9/pytextclassifier/fasttext_classifier.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 pytextclassifier-1.3.9/pytextclassifier/stopwords.txt
+-rw-r--r--   0 xuming     (501) staff       (20)     7304 2023-05-09 08:44:44.000000 pytextclassifier-1.3.9/pytextclassifier/textcluster.py
+-rw-r--r--   0 xuming     (501) staff       (20)    19072 2023-10-18 04:11:21.000000 pytextclassifier-1.3.9/pytextclassifier/textcnn_classifier.py
+-rw-r--r--   0 xuming     (501) staff       (20)    19709 2023-10-18 04:11:21.000000 pytextclassifier-1.3.9/pytextclassifier/textrnn_classifier.py
+-rw-r--r--   0 xuming     (501) staff       (20)      852 2022-04-12 06:51:36.000000 pytextclassifier-1.3.9/pytextclassifier/time_util.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2331 2023-06-14 12:38:54.000000 pytextclassifier-1.3.9/pytextclassifier/tokenizer.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-05-22 03:33:52.913466 pytextclassifier-1.3.9/pytextclassifier.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    22590 2024-05-22 03:33:52.000000 pytextclassifier-1.3.9/pytextclassifier.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)      848 2024-05-22 03:33:52.000000 pytextclassifier-1.3.9/pytextclassifier.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2024-05-22 03:33:52.000000 pytextclassifier-1.3.9/pytextclassifier.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)       52 2024-05-22 03:33:52.000000 pytextclassifier-1.3.9/pytextclassifier.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)       17 2024-05-22 03:33:52.000000 pytextclassifier-1.3.9/pytextclassifier.egg-info/top_level.txt
+-rw-r--r--   0 xuming     (501) staff       (20)      309 2024-05-22 03:33:52.920605 pytextclassifier-1.3.9/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1444 2024-05-22 03:31:13.000000 pytextclassifier-1.3.9/setup.py
```

### Comparing `pytextclassifier-1.3.8/LICENSE` & `pytextclassifier-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/PKG-INFO` & `pytextclassifier-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytextclassifier
-Version: 1.3.8
+Version: 1.3.9
 Summary: Text Classifier, Text Classification
 Home-page: https://github.com/shibing624/pytextclassifier
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Keywords: pytextclassifier,textclassifier,classifier,textclassification
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pytextclassifier-1.3.8/README.md` & `pytextclassifier-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/examples/thucnews_train_1w.txt` & `pytextclassifier-1.3.9/examples/thucnews_train_1w.txt`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/pytextclassifier/__init__.py` & `pytextclassifier-1.3.9/pytextclassifier/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
-__version__ = '1.3.8'
+__version__ = '1.3.9'
 
 from pytextclassifier.classic_classifier import ClassicClassifier
 from pytextclassifier.fasttext_classifier import FastTextClassifier
 from pytextclassifier.textcnn_classifier import TextCNNClassifier
 from pytextclassifier.textrnn_classifier import TextRNNClassifier
 from pytextclassifier.bert_classifier import BertClassifier
 from pytextclassifier.base_classifier import load_data
```

### Comparing `pytextclassifier-1.3.8/pytextclassifier/base_classifier.py` & `pytextclassifier-1.3.9/pytextclassifier/base_classifier.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/pytextclassifier/bert_classfication_utils.py` & `pytextclassifier-1.3.9/pytextclassifier/bert_classfication_utils.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/pytextclassifier/bert_classification_model.py` & `pytextclassifier-1.3.9/pytextclassifier/bert_classification_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,82 +62,70 @@
     XLMForSequenceClassification,
     XLNetTokenizerFast,
     XLNetForSequenceClassification,
     BertConfig,
     BertTokenizer,
     BertweetTokenizer,
     DistilBertConfig,
-    DistilBertTokenizer,
     ElectraConfig,
-    ElectraTokenizer,
     HerbertTokenizer,
     LongformerConfig,
     LongformerTokenizer,
     RobertaConfig,
-    RobertaTokenizer,
     XLMConfig,
     XLMRobertaConfig,
-    XLMRobertaTokenizer,
     XLMTokenizer,
     XLNetConfig,
     XLNetTokenizer,
 )
 from transformers.convert_graph_to_onnx import convert, quantize
 from transformers.optimization import AdamW, Adafactor
 from transformers.optimization import (
     get_constant_schedule,
     get_constant_schedule_with_warmup,
     get_linear_schedule_with_warmup,
     get_cosine_schedule_with_warmup,
     get_cosine_with_hard_restarts_schedule_with_warmup,
     get_polynomial_decay_schedule_with_warmup,
 )
+
 sys.path.append('..')
 from pytextclassifier.bert_classfication_utils import (
     BertClassificationArgs,
     InputExample,
     LazyClassificationDataset,
     ClassificationDataset,
     load_hf_dataset,
     flatten_results,
     init_loss,
 )
 from pytextclassifier.bert_multi_label_classification_model import (
     AlbertForMultiLabelSequenceClassification,
     BertForMultiLabelSequenceClassification,
-    BertweetForMultiLabelSequenceClassification,
-    DistilBertForMultiLabelSequenceClassification,
-    ElectraForMultiLabelSequenceClassification,
     LongformerForMultiLabelSequenceClassification,
-    RobertaForMultiLabelSequenceClassification,
     XLMForMultiLabelSequenceClassification,
-    XLMRobertaForMultiLabelSequenceClassification,
     XLNetForMultiLabelSequenceClassification
 )
 
 try:
     import wandb
 
     wandb_available = True
 except ImportError:
     wandb_available = False
 
 MODELS_WITHOUT_CLASS_WEIGHTS_SUPPORT = ["deberta", "mpnet"]
 
 MODELS_WITH_EXTRA_SEP_TOKEN = [
-    "roberta",
-    "camembert",
     "xlmroberta",
     "longformer",
     "mpnet",
 ]
 
 MODELS_WITH_ADD_PREFIX_SPACE = [
-    "roberta",
-    "camembert",
     "xlmroberta",
     "longformer",
     "mpnet",
 ]
 
 
 class BertClassificationModel:
@@ -183,50 +171,25 @@
                     AutoTokenizer,
                 ),
                 "bert": (
                     BertConfig,
                     BertForMultiLabelSequenceClassification,
                     BertTokenizer,
                 ),
-                "bertweet": (
-                    RobertaConfig,
-                    BertweetForMultiLabelSequenceClassification,
-                    BertweetTokenizer,
-                ),
-                "distilbert": (
-                    DistilBertConfig,
-                    DistilBertForMultiLabelSequenceClassification,
-                    DistilBertTokenizer,
-                ),
-                "electra": (
-                    ElectraConfig,
-                    ElectraForMultiLabelSequenceClassification,
-                    ElectraTokenizer,
-                ),
                 "herbert": (
                     BertConfig,
                     BertForMultiLabelSequenceClassification,
                     HerbertTokenizer,
                 ),
                 "longformer": (
                     LongformerConfig,
                     LongformerForMultiLabelSequenceClassification,
                     LongformerTokenizer,
                 ),
-                "roberta": (
-                    RobertaConfig,
-                    RobertaForMultiLabelSequenceClassification,
-                    RobertaTokenizer,
-                ),
                 "xlm": (XLMConfig, XLMForMultiLabelSequenceClassification, XLMTokenizer),
-                "xlmroberta": (
-                    XLMRobertaConfig,
-                    XLMRobertaForMultiLabelSequenceClassification,
-                    XLMRobertaTokenizer,
-                ),
                 "xlnet": (
                     XLNetConfig,
                     XLNetForMultiLabelSequenceClassification,
                     XLNetTokenizer,
                 ),
             }
         else:
```

### Comparing `pytextclassifier-1.3.8/pytextclassifier/bert_classifier.py` & `pytextclassifier-1.3.9/pytextclassifier/bert_classifier.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/pytextclassifier/classic_classifier.py` & `pytextclassifier-1.3.9/pytextclassifier/classic_classifier.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/pytextclassifier/data_helper.py` & `pytextclassifier-1.3.9/pytextclassifier/data_helper.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/pytextclassifier/fasttext_classifier.py` & `pytextclassifier-1.3.9/pytextclassifier/fasttext_classifier.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/pytextclassifier/stopwords.txt` & `pytextclassifier-1.3.9/pytextclassifier/stopwords.txt`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/pytextclassifier/textcluster.py` & `pytextclassifier-1.3.9/pytextclassifier/textcluster.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/pytextclassifier/textcnn_classifier.py` & `pytextclassifier-1.3.9/pytextclassifier/textcnn_classifier.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/pytextclassifier/textrnn_classifier.py` & `pytextclassifier-1.3.9/pytextclassifier/textrnn_classifier.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/pytextclassifier/time_util.py` & `pytextclassifier-1.3.9/pytextclassifier/time_util.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/pytextclassifier/tokenizer.py` & `pytextclassifier-1.3.9/pytextclassifier/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/pytextclassifier.egg-info/PKG-INFO` & `pytextclassifier-1.3.9/pytextclassifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytextclassifier
-Version: 1.3.8
+Version: 1.3.9
 Summary: Text Classifier, Text Classification
 Home-page: https://github.com/shibing624/pytextclassifier
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Keywords: pytextclassifier,textclassifier,classifier,textclassification
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pytextclassifier-1.3.8/pytextclassifier.egg-info/SOURCES.txt` & `pytextclassifier-1.3.9/pytextclassifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.8/setup.py` & `pytextclassifier-1.3.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
 from setuptools import setup, find_packages
 
-__version__ = '1.3.8'
+__version__ = '1.3.9'
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='pytextclassifier',
     version=__version__,
```

