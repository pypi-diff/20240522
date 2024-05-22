# Comparing `tmp/billm-0.1.3.tar.gz` & `tmp/billm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "billm-0.1.3.tar", last modified: Sun Apr  7 03:32:34 2024, max compression
+gzip compressed data, was "billm-0.1.4.tar", last modified: Wed May 22 08:36:43 2024, max compression
```

## Comparing `billm-0.1.3.tar` & `billm-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1060 2024-03-14 10:50:27.655921 billm-0.1.3/LICENSE
--rw-r--r--   0        0        0     4216 2024-04-07 03:30:51.080529 billm-0.1.3/README.md
--rw-r--r--   0        0        0      486 2024-04-07 03:32:34.911507 billm-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      165 2024-04-07 03:31:24.729919 billm-0.1.3/src/billm/__init__.py
--rw-r--r--   0        0        0      267 2024-03-17 05:50:48.094383 billm-0.1.3/src/billm/config.py
--rw-r--r--   0        0        0    29171 2024-04-07 03:30:51.083126 billm-0.1.3/src/billm/modeling_llama.py
--rw-r--r--   0        0        0    25668 2024-04-07 03:30:51.084231 billm-0.1.3/src/billm/modeling_mistral.py
--rw-r--r--   0        0        0    25464 2024-04-07 03:30:51.085109 billm-0.1.3/src/billm/modeling_qwen2.py
--rw-r--r--   0        0        0        0 2024-03-17 05:50:48.095776 billm-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     2598 2024-04-07 03:30:51.086211 billm-0.1.3/tests/test_modeling_llama.py
--rw-r--r--   0        0        0     2728 2024-04-07 03:30:51.087077 billm-0.1.3/tests/test_modeling_mistral.py
--rw-r--r--   0        0        0     2678 2024-04-07 03:30:51.087923 billm-0.1.3/tests/test_modeling_qwen2.py
--rw-r--r--   0        0        0     4549 1970-01-01 00:00:00.000000 billm-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-03-14 10:50:27.655921 billm-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4352 2024-05-22 08:34:53.290584 billm-0.1.4/README.md
+-rw-r--r--   0        0        0      486 2024-05-22 08:36:43.224875 billm-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      205 2024-05-22 08:35:50.555270 billm-0.1.4/src/billm/__init__.py
+-rw-r--r--   0        0        0      267 2024-03-17 05:50:48.094383 billm-0.1.4/src/billm/config.py
+-rw-r--r--   0        0        0    14376 2024-05-22 08:34:53.296221 billm-0.1.4/src/billm/configuration_openelm.py
+-rw-r--r--   0        0        0    29160 2024-05-22 08:34:53.299901 billm-0.1.4/src/billm/modeling_llama.py
+-rw-r--r--   0        0        0    25657 2024-05-22 08:34:53.302473 billm-0.1.4/src/billm/modeling_mistral.py
+-rw-r--r--   0        0        0    47882 2024-05-22 08:34:53.306016 billm-0.1.4/src/billm/modeling_openelm.py
+-rw-r--r--   0        0        0    25453 2024-05-22 08:34:53.308417 billm-0.1.4/src/billm/modeling_qwen2.py
+-rw-r--r--   0        0        0        0 2024-03-17 05:50:48.095776 billm-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     2598 2024-04-07 03:30:51.086211 billm-0.1.4/tests/test_modeling_llama.py
+-rw-r--r--   0        0        0     2728 2024-04-07 03:30:51.087077 billm-0.1.4/tests/test_modeling_mistral.py
+-rw-r--r--   0        0        0     2037 2024-05-22 08:34:53.311395 billm-0.1.4/tests/test_modeling_openelm.py
+-rw-r--r--   0        0        0     2678 2024-04-07 03:30:51.087923 billm-0.1.4/tests/test_modeling_qwen2.py
+-rw-r--r--   0        0        0     4685 1970-01-01 00:00:00.000000 billm-0.1.4/PKG-INFO
```

### Comparing `billm-0.1.3/LICENSE` & `billm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `billm-0.1.3/README.md` & `billm-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,18 @@
 +    MistralForCausalLM,
 +    MistralForSequenceClassification,
 +    MistralForTokenClassification,
 +    Qwen2Model,
 +    Qwen2ForCausalLM,
 +    Qwen2ForSequenceClassification,
 +    Qwen2ForTokenClassification
++    OpenELMModel,
++    OpenELMForCausalLM,
++    OpenELMForSequenceClassification,
++    OpenELMForTokenClassification
 + )
 ```
 
 ## Examples
 
 ### NER
 
@@ -100,14 +104,16 @@
 ```
 
 
 ## Supported Models
 
 - LLaMA
 - Mistral
+- Qwen2
+- OpenELM
 
 ## Citation
 
 If you use this toolkit in your work, please cite the following paper:
 
 1) For sentence embeddings modeling:
```

#### html2text {}

```diff
@@ -10,37 +10,38 @@
 LLamaForCausalLM, - LLamaForSequenceClassification, - MistralModel, -
 MistralForCausalLM, - MistralForSequenceClassification - Qwen2Model, -
 Qwen2ForCausalLM, - Qwen2ForSequenceClassification - ) + from billm import ( +
 LLamaModel, + LLamaForCausalLM, + LLamaForSequenceClassification, +
 LLamaForTokenClassification, + MistralModel, + MistralForCausalLM, +
 MistralForSequenceClassification, + MistralForTokenClassification, +
 Qwen2Model, + Qwen2ForCausalLM, + Qwen2ForSequenceClassification, +
-Qwen2ForTokenClassification + ) ``` ## Examples ### NER **training:** ```bash $
-cd examples $ WANDB_MODE=disabled BiLLM_START_INDEX=0 CUDA_VISIBLE_DEVICES=3
-python billm_ner.py \ --model_name_or_path mistralai/Mistral-7B-v0.1 \ --
-dataset_name_or_path conll2003 \ --push_to_hub 0 ``` **inference:** ```python
-from transformers import AutoTokenizer, pipeline from peft import PeftModel,
-PeftConfig from billm import MistralForTokenClassification label2id = {'O': 0,
-'B-PER': 1, 'I-PER': 2, 'B-ORG': 3, 'I-ORG': 4, 'B-LOC': 5, 'I-LOC': 6, 'B-
-MISC': 7, 'I-MISC': 8} id2label = {v: k for k, v in label2id.items()} model_id
-= 'WhereIsAI/billm-mistral-7b-conll03-ner' tokenizer =
-AutoTokenizer.from_pretrained(model_id) peft_config =
-PeftConfig.from_pretrained(model_id) model =
+Qwen2ForTokenClassification + OpenELMModel, + OpenELMForCausalLM, +
+OpenELMForSequenceClassification, + OpenELMForTokenClassification + ) ``` ##
+Examples ### NER **training:** ```bash $ cd examples $ WANDB_MODE=disabled
+BiLLM_START_INDEX=0 CUDA_VISIBLE_DEVICES=3 python billm_ner.py \ --
+model_name_or_path mistralai/Mistral-7B-v0.1 \ --dataset_name_or_path conll2003
+\ --push_to_hub 0 ``` **inference:** ```python from transformers import
+AutoTokenizer, pipeline from peft import PeftModel, PeftConfig from billm
+import MistralForTokenClassification label2id = {'O': 0, 'B-PER': 1, 'I-PER':
+2, 'B-ORG': 3, 'I-ORG': 4, 'B-LOC': 5, 'I-LOC': 6, 'B-MISC': 7, 'I-MISC': 8}
+id2label = {v: k for k, v in label2id.items()} model_id = 'WhereIsAI/billm-
+mistral-7b-conll03-ner' tokenizer = AutoTokenizer.from_pretrained(model_id)
+peft_config = PeftConfig.from_pretrained(model_id) model =
 MistralForTokenClassification.from_pretrained
 ( peft_config.base_model_name_or_path, num_labels=len(label2id),
 id2label=id2label, label2id=label2id ) model = PeftModel.from_pretrained(model,
 model_id) # merge and unload is necessary for inference model =
 model.merge_and_unload() token_classifier = pipeline("token-classification",
 model=model, tokenizer=tokenizer, aggregation_strategy="simple") sentence = "I
 live in Hong Kong. I am a student at Hong Kong PolyU." tokens =
 token_classifier(sentence) print(tokens) ``` ## Supported Models - LLaMA -
-Mistral ## Citation If you use this toolkit in your work, please cite the
-following paper: 1) For sentence embeddings modeling: ```bibtex @inproceedings
-{li2024bellm, title = "BeLLM: Backward Dependency Enhanced Large Language Model
-for Sentence Embeddings", author = "Li, Xianming and Li, Jing", booktitle =
-"Proceedings of the 2024 Conference of the North American Chapter of the
-Association for Computational Linguistics", year = "2024", publisher =
+Mistral - Qwen2 - OpenELM ## Citation If you use this toolkit in your work,
+please cite the following paper: 1) For sentence embeddings modeling: ```bibtex
+@inproceedings{li2024bellm, title = "BeLLM: Backward Dependency Enhanced Large
+Language Model for Sentence Embeddings", author = "Li, Xianming and Li, Jing",
+booktitle = "Proceedings of the 2024 Conference of the North American Chapter
+of the Association for Computational Linguistics", year = "2024", publisher =
 "Association for Computational Linguistics" } ``` 2) For other tasks: ```bibtex
 @article{li2023label, title={Label supervised llama finetuning}, author={Li,
 Zongxi and Li, Xianming and Liu, Yuzhang and Xie, Haoran and Li, Jing and Wang,
 Fu-lee and Li, Qing and Zhong, Xiaoqin}, journal={arXiv preprint arXiv:
 2310.01208}, year={2023} } ```
```

### Comparing `billm-0.1.3/src/billm/modeling_llama.py` & `billm-0.1.4/src/billm/modeling_llama.py`

 * *Files 0% similar despite different names*

```diff
@@ -479,15 +479,15 @@
         past_key_values: Optional[List[torch.FloatTensor]] = None,
         inputs_embeds: Optional[torch.FloatTensor] = None,
         labels: Optional[torch.LongTensor] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
-    ) -> Union[Tuple, SequenceClassifierOutputWithPast]:
+    ) -> Union[Tuple, TokenClassifierOutput]:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
             Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
             config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
             `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
         """
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
```

### Comparing `billm-0.1.3/src/billm/modeling_mistral.py` & `billm-0.1.4/src/billm/modeling_mistral.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
         past_key_values: Optional[List[torch.FloatTensor]] = None,
         inputs_embeds: Optional[torch.FloatTensor] = None,
         labels: Optional[torch.LongTensor] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
-    ) -> Union[Tuple, SequenceClassifierOutputWithPast]:
+    ) -> Union[Tuple, TokenClassifierOutput]:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
             Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
             config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
             `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
         """
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
```

### Comparing `billm-0.1.3/src/billm/modeling_qwen2.py` & `billm-0.1.4/src/billm/modeling_qwen2.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,15 +546,15 @@
         past_key_values: Optional[List[torch.FloatTensor]] = None,
         inputs_embeds: Optional[torch.FloatTensor] = None,
         labels: Optional[torch.LongTensor] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
-    ) -> Union[Tuple, SequenceClassifierOutputWithPast]:
+    ) -> Union[Tuple, TokenClassifierOutput]:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
             Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
             config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
             `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
         """
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
```

### Comparing `billm-0.1.3/tests/test_modeling_llama.py` & `billm-0.1.4/tests/test_modeling_llama.py`

 * *Files identical despite different names*

### Comparing `billm-0.1.3/tests/test_modeling_mistral.py` & `billm-0.1.4/tests/test_modeling_mistral.py`

 * *Files identical despite different names*

### Comparing `billm-0.1.3/tests/test_modeling_qwen2.py` & `billm-0.1.4/tests/test_modeling_qwen2.py`

 * *Files identical despite different names*

### Comparing `billm-0.1.3/PKG-INFO` & `billm-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BiLLM
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tool for converting LLMs from uni-directional to bi-directional for tasks like classification and sentence embeddings.
 Author-Email: Sean Lee <xmlee97@gmail.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: transformers>=4.38.2
 Description-Content-Type: text/markdown
 
@@ -61,14 +61,18 @@
 +    MistralForCausalLM,
 +    MistralForSequenceClassification,
 +    MistralForTokenClassification,
 +    Qwen2Model,
 +    Qwen2ForCausalLM,
 +    Qwen2ForSequenceClassification,
 +    Qwen2ForTokenClassification
++    OpenELMModel,
++    OpenELMForCausalLM,
++    OpenELMForSequenceClassification,
++    OpenELMForTokenClassification
 + )
 ```
 
 ## Examples
 
 ### NER
 
@@ -110,14 +114,16 @@
 ```
 
 
 ## Supported Models
 
 - LLaMA
 - Mistral
+- Qwen2
+- OpenELM
 
 ## Citation
 
 If you use this toolkit in your work, please cite the following paper:
 
 1) For sentence embeddings modeling:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BiLLM Version: 0.1.3 Summary: Tool for converting
+Metadata-Version: 2.1 Name: BiLLM Version: 0.1.4 Summary: Tool for converting
 LLMs from uni-directional to bi-directional for tasks like classification and
 sentence embeddings. Author-Email: Sean Lee
 gmail.com> License: MIT Requires-Python: >=3.8 Requires-Dist:
 transformers>=4.38.2 Description-Content-Type: text/markdown # BiLLM Tool for
 converting LLMs from uni-directional to bi-directional for tasks like
 classification and sentence embeddings. Compatible with ð¤ transformers.
 _[_h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_3_1_0_._0_1_2_0_8_]_[_h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_3_1_1_._0_5_2_9_6_]_[_P_y_P_I
@@ -15,37 +15,38 @@
 LLamaForCausalLM, - LLamaForSequenceClassification, - MistralModel, -
 MistralForCausalLM, - MistralForSequenceClassification - Qwen2Model, -
 Qwen2ForCausalLM, - Qwen2ForSequenceClassification - ) + from billm import ( +
 LLamaModel, + LLamaForCausalLM, + LLamaForSequenceClassification, +
 LLamaForTokenClassification, + MistralModel, + MistralForCausalLM, +
 MistralForSequenceClassification, + MistralForTokenClassification, +
 Qwen2Model, + Qwen2ForCausalLM, + Qwen2ForSequenceClassification, +
-Qwen2ForTokenClassification + ) ``` ## Examples ### NER **training:** ```bash $
-cd examples $ WANDB_MODE=disabled BiLLM_START_INDEX=0 CUDA_VISIBLE_DEVICES=3
-python billm_ner.py \ --model_name_or_path mistralai/Mistral-7B-v0.1 \ --
-dataset_name_or_path conll2003 \ --push_to_hub 0 ``` **inference:** ```python
-from transformers import AutoTokenizer, pipeline from peft import PeftModel,
-PeftConfig from billm import MistralForTokenClassification label2id = {'O': 0,
-'B-PER': 1, 'I-PER': 2, 'B-ORG': 3, 'I-ORG': 4, 'B-LOC': 5, 'I-LOC': 6, 'B-
-MISC': 7, 'I-MISC': 8} id2label = {v: k for k, v in label2id.items()} model_id
-= 'WhereIsAI/billm-mistral-7b-conll03-ner' tokenizer =
-AutoTokenizer.from_pretrained(model_id) peft_config =
-PeftConfig.from_pretrained(model_id) model =
+Qwen2ForTokenClassification + OpenELMModel, + OpenELMForCausalLM, +
+OpenELMForSequenceClassification, + OpenELMForTokenClassification + ) ``` ##
+Examples ### NER **training:** ```bash $ cd examples $ WANDB_MODE=disabled
+BiLLM_START_INDEX=0 CUDA_VISIBLE_DEVICES=3 python billm_ner.py \ --
+model_name_or_path mistralai/Mistral-7B-v0.1 \ --dataset_name_or_path conll2003
+\ --push_to_hub 0 ``` **inference:** ```python from transformers import
+AutoTokenizer, pipeline from peft import PeftModel, PeftConfig from billm
+import MistralForTokenClassification label2id = {'O': 0, 'B-PER': 1, 'I-PER':
+2, 'B-ORG': 3, 'I-ORG': 4, 'B-LOC': 5, 'I-LOC': 6, 'B-MISC': 7, 'I-MISC': 8}
+id2label = {v: k for k, v in label2id.items()} model_id = 'WhereIsAI/billm-
+mistral-7b-conll03-ner' tokenizer = AutoTokenizer.from_pretrained(model_id)
+peft_config = PeftConfig.from_pretrained(model_id) model =
 MistralForTokenClassification.from_pretrained
 ( peft_config.base_model_name_or_path, num_labels=len(label2id),
 id2label=id2label, label2id=label2id ) model = PeftModel.from_pretrained(model,
 model_id) # merge and unload is necessary for inference model =
 model.merge_and_unload() token_classifier = pipeline("token-classification",
 model=model, tokenizer=tokenizer, aggregation_strategy="simple") sentence = "I
 live in Hong Kong. I am a student at Hong Kong PolyU." tokens =
 token_classifier(sentence) print(tokens) ``` ## Supported Models - LLaMA -
-Mistral ## Citation If you use this toolkit in your work, please cite the
-following paper: 1) For sentence embeddings modeling: ```bibtex @inproceedings
-{li2024bellm, title = "BeLLM: Backward Dependency Enhanced Large Language Model
-for Sentence Embeddings", author = "Li, Xianming and Li, Jing", booktitle =
-"Proceedings of the 2024 Conference of the North American Chapter of the
-Association for Computational Linguistics", year = "2024", publisher =
+Mistral - Qwen2 - OpenELM ## Citation If you use this toolkit in your work,
+please cite the following paper: 1) For sentence embeddings modeling: ```bibtex
+@inproceedings{li2024bellm, title = "BeLLM: Backward Dependency Enhanced Large
+Language Model for Sentence Embeddings", author = "Li, Xianming and Li, Jing",
+booktitle = "Proceedings of the 2024 Conference of the North American Chapter
+of the Association for Computational Linguistics", year = "2024", publisher =
 "Association for Computational Linguistics" } ``` 2) For other tasks: ```bibtex
 @article{li2023label, title={Label supervised llama finetuning}, author={Li,
 Zongxi and Li, Xianming and Liu, Yuzhang and Xie, Haoran and Li, Jing and Wang,
 Fu-lee and Li, Qing and Zhong, Xiaoqin}, journal={arXiv preprint arXiv:
 2310.01208}, year={2023} } ```
```

