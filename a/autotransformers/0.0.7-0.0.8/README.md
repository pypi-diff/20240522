# Comparing `tmp/autotransformers-0.0.7.tar.gz` & `tmp/autotransformers-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotransformers-0.0.7.tar", max compression
+gzip compressed data, was "autotransformers-0.0.8.tar", max compression
```

## Comparing `autotransformers-0.0.7.tar` & `autotransformers-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rwxr-xr-x   0        0        0    20849 2024-03-12 18:46:16.934454 autotransformers-0.0.7/LICENSE
--rwxr-xr-x   0        0        0    23693 2024-03-18 10:32:51.314243 autotransformers-0.0.7/README.md
--rwxr-xr-x   0        0        0     2029 2024-03-18 13:26:31.929865 autotransformers-0.0.7/pyproject.toml
--rwxr-xr-x   0        0        0      661 2024-03-12 18:46:17.645952 autotransformers-0.0.7/src/autotransformers/__init__.py
--rwxr-xr-x   0        0        0     2916 2024-03-12 18:46:17.621950 autotransformers-0.0.7/src/autotransformers/augmentation/TextAugmenterPipeline.py
--rwxr-xr-x   0        0        0       93 2024-03-12 18:46:17.541017 autotransformers-0.0.7/src/autotransformers/augmentation/__init__.py
--rwxr-xr-x   0        0        0     3319 2024-03-17 08:31:17.168382 autotransformers-0.0.7/src/autotransformers/augmentation/__pycache__/TextAugmenterPipeline.cpython-310.pyc
--rwxr-xr-x   0        0        0     5050 2024-03-12 20:27:43.949710 autotransformers-0.0.7/src/autotransformers/augmentation/__pycache__/TextAugmenterPipeline.cpython-311.pyc
--rwxr-xr-x   0        0        0      299 2024-03-17 08:31:14.854249 autotransformers-0.0.7/src/autotransformers/augmentation/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      345 2024-03-12 20:27:39.617320 autotransformers-0.0.7/src/autotransformers/augmentation/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     2595 2024-03-17 08:31:14.883397 autotransformers-0.0.7/src/autotransformers/augmentation/__pycache__/augmenter_config.cpython-310.pyc
--rwxr-xr-x   0        0        0     3249 2024-03-12 20:27:39.639763 autotransformers-0.0.7/src/autotransformers/augmentation/__pycache__/augmenter_config.cpython-311.pyc
--rwxr-xr-x   0        0        0     2250 2024-03-12 18:46:17.628948 autotransformers-0.0.7/src/autotransformers/augmentation/augmenter_config.py
--rwxr-xr-x   0        0        0    23039 2024-03-17 10:21:51.652847 autotransformers-0.0.7/src/autotransformers/autotrainer.py
--rwxr-xr-x   0        0        0     7699 2024-03-12 18:46:17.504062 autotransformers-0.0.7/src/autotransformers/ckpt_cleaner.py
--rwxr-xr-x   0        0        0    13988 2024-03-12 18:46:17.499063 autotransformers-0.0.7/src/autotransformers/dataset_config.py
--rwxr-xr-x   0        0        0     2043 2024-03-12 18:46:17.518064 autotransformers-0.0.7/src/autotransformers/default_param_spaces.py
--rwxr-xr-x   0        0        0    11576 2024-03-17 09:35:19.635531 autotransformers-0.0.7/src/autotransformers/hfdatasets_manager.py
--rwxr-xr-x   0        0        0    16416 2024-03-16 13:14:15.446975 autotransformers-0.0.7/src/autotransformers/hftransformers_manager.py
--rwxr-xr-x   0        0        0    19342 2024-03-18 13:24:35.931973 autotransformers-0.0.7/src/autotransformers/llm_templates.py
--rwxr-xr-x   0        0        0     6323 2024-03-12 18:46:17.509064 autotransformers-0.0.7/src/autotransformers/metrics.py
--rwxr-xr-x   0        0        0     6058 2024-03-14 07:58:10.558200 autotransformers-0.0.7/src/autotransformers/metrics_plotter.py
--rwxr-xr-x   0        0        0    12504 2024-03-14 07:58:10.612207 autotransformers-0.0.7/src/autotransformers/model_config.py
--rwxr-xr-x   0        0        0    17301 2024-03-12 18:46:17.529066 autotransformers-0.0.7/src/autotransformers/results_getter.py
--rwxr-xr-x   0        0        0      488 2024-03-12 18:46:17.953352 autotransformers-0.0.7/src/autotransformers/skip_mix.py
--rwxr-xr-x   0        0        0    10828 2024-03-12 18:46:17.523066 autotransformers-0.0.7/src/autotransformers/tokenization_functions.py
--rwxr-xr-x   0        0        0    13527 2024-03-13 09:39:38.658801 autotransformers-0.0.7/src/autotransformers/utils.py
--rw-r--r--   0        0        0    25892 1970-01-01 00:00:00.000000 autotransformers-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0    20849 2024-03-12 18:46:16.934454 autotransformers-0.0.8/LICENSE
+-rwxr-xr-x   0        0        0    23996 2024-04-22 07:35:17.996309 autotransformers-0.0.8/README.md
+-rwxr-xr-x   0        0        0     2029 2024-05-22 18:15:10.668489 autotransformers-0.0.8/pyproject.toml
+-rwxr-xr-x   0        0        0      661 2024-03-12 18:46:17.645952 autotransformers-0.0.8/src/autotransformers/__init__.py
+-rwxr-xr-x   0        0        0     2916 2024-03-12 18:46:17.621950 autotransformers-0.0.8/src/autotransformers/augmentation/TextAugmenterPipeline.py
+-rwxr-xr-x   0        0        0       93 2024-03-12 18:46:17.541017 autotransformers-0.0.8/src/autotransformers/augmentation/__init__.py
+-rwxr-xr-x   0        0        0     3319 2024-03-17 08:31:17.168382 autotransformers-0.0.8/src/autotransformers/augmentation/__pycache__/TextAugmenterPipeline.cpython-310.pyc
+-rwxr-xr-x   0        0        0     5050 2024-03-12 20:27:43.949710 autotransformers-0.0.8/src/autotransformers/augmentation/__pycache__/TextAugmenterPipeline.cpython-311.pyc
+-rwxr-xr-x   0        0        0      299 2024-03-17 08:31:14.854249 autotransformers-0.0.8/src/autotransformers/augmentation/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      345 2024-03-12 20:27:39.617320 autotransformers-0.0.8/src/autotransformers/augmentation/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2595 2024-03-17 08:31:14.883397 autotransformers-0.0.8/src/autotransformers/augmentation/__pycache__/augmenter_config.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3249 2024-03-12 20:27:39.639763 autotransformers-0.0.8/src/autotransformers/augmentation/__pycache__/augmenter_config.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2250 2024-03-12 18:46:17.628948 autotransformers-0.0.8/src/autotransformers/augmentation/augmenter_config.py
+-rwxr-xr-x   0        0        0    23039 2024-03-17 10:21:51.652847 autotransformers-0.0.8/src/autotransformers/autotrainer.py
+-rwxr-xr-x   0        0        0     7699 2024-03-12 18:46:17.504062 autotransformers-0.0.8/src/autotransformers/ckpt_cleaner.py
+-rwxr-xr-x   0        0        0    13988 2024-03-12 18:46:17.499063 autotransformers-0.0.8/src/autotransformers/dataset_config.py
+-rwxr-xr-x   0        0        0     2043 2024-03-12 18:46:17.518064 autotransformers-0.0.8/src/autotransformers/default_param_spaces.py
+-rwxr-xr-x   0        0        0    11576 2024-03-17 09:35:19.635531 autotransformers-0.0.8/src/autotransformers/hfdatasets_manager.py
+-rwxr-xr-x   0        0        0    16416 2024-03-16 13:14:15.446975 autotransformers-0.0.8/src/autotransformers/hftransformers_manager.py
+-rwxr-xr-x   0        0        0    19342 2024-03-18 13:24:35.931973 autotransformers-0.0.8/src/autotransformers/llm_templates.py
+-rwxr-xr-x   0        0        0     6317 2024-05-22 09:13:54.464921 autotransformers-0.0.8/src/autotransformers/metrics.py
+-rwxr-xr-x   0        0        0     6058 2024-03-14 07:58:10.558200 autotransformers-0.0.8/src/autotransformers/metrics_plotter.py
+-rwxr-xr-x   0        0        0    12504 2024-03-14 07:58:10.612207 autotransformers-0.0.8/src/autotransformers/model_config.py
+-rwxr-xr-x   0        0        0    17301 2024-03-12 18:46:17.529066 autotransformers-0.0.8/src/autotransformers/results_getter.py
+-rwxr-xr-x   0        0        0      488 2024-03-12 18:46:17.953352 autotransformers-0.0.8/src/autotransformers/skip_mix.py
+-rwxr-xr-x   0        0        0    10828 2024-03-12 18:46:17.523066 autotransformers-0.0.8/src/autotransformers/tokenization_functions.py
+-rwxr-xr-x   0        0        0    13527 2024-03-13 09:39:38.658801 autotransformers-0.0.8/src/autotransformers/utils.py
+-rw-r--r--   0        0        0    26195 1970-01-01 00:00:00.000000 autotransformers-0.0.8/PKG-INFO
```

### Comparing `autotransformers-0.0.7/LICENSE` & `autotransformers-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/README.md` & `autotransformers-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -399,8 +399,19 @@
     model_configs = [model_config],
     dataset_configs = [data_config]
 )
 
 autotrainer()
 ```
 
-In this way, we are using the pipeline to internally augment data before training, therefore we will increment the amount of training data, without modifying the validation and test subsets.
+In this way, we are using the pipeline to internally augment data before training, therefore we will increment the amount of training data, without modifying the validation and test subsets.
+
+## Citation
+
+```
+@misc{vaca2024autotransformers,
+    author = {Alejandro Vaca Serrano},
+    title = {AutoTransformers: A Library for Automatic Training and Benchmarking of Transformer Models},
+    year = {2024},
+    howpublished = {\url{https://github.com/lenguajenatural-ai/autotransformers}},
+}
+```
```

### Comparing `autotransformers-0.0.7/pyproject.toml` & `autotransformers-0.0.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autotransformers"
-version = "0.0.7"
+version = "0.0.8"
 description = "a Python package for automatic training and benchmarking of Language Models."
 authors = [
     "LenguajeNatural.AI <avaca@lenguajenatural.ai>"
 ]
 license = "CC BY-NC-SA 4.0"
 readme = "README.md"
 homepage = "https://lenguajenatural.ai"
```

### Comparing `autotransformers-0.0.7/src/autotransformers/__init__.py` & `autotransformers-0.0.8/src/autotransformers/__init__.py`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/augmentation/TextAugmenterPipeline.py` & `autotransformers-0.0.8/src/autotransformers/augmentation/TextAugmenterPipeline.py`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/augmentation/__pycache__/TextAugmenterPipeline.cpython-310.pyc` & `autotransformers-0.0.8/src/autotransformers/augmentation/__pycache__/TextAugmenterPipeline.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/augmentation/__pycache__/TextAugmenterPipeline.cpython-311.pyc` & `autotransformers-0.0.8/src/autotransformers/augmentation/__pycache__/TextAugmenterPipeline.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/augmentation/__pycache__/augmenter_config.cpython-310.pyc` & `autotransformers-0.0.8/src/autotransformers/augmentation/__pycache__/augmenter_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/augmentation/__pycache__/augmenter_config.cpython-311.pyc` & `autotransformers-0.0.8/src/autotransformers/augmentation/__pycache__/augmenter_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/augmentation/augmenter_config.py` & `autotransformers-0.0.8/src/autotransformers/augmentation/augmenter_config.py`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/autotrainer.py` & `autotransformers-0.0.8/src/autotransformers/autotrainer.py`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/ckpt_cleaner.py` & `autotransformers-0.0.8/src/autotransformers/ckpt_cleaner.py`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/dataset_config.py` & `autotransformers-0.0.8/src/autotransformers/dataset_config.py`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/default_param_spaces.py` & `autotransformers-0.0.8/src/autotransformers/default_param_spaces.py`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/hfdatasets_manager.py` & `autotransformers-0.0.8/src/autotransformers/hfdatasets_manager.py`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/hftransformers_manager.py` & `autotransformers-0.0.8/src/autotransformers/hftransformers_manager.py`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/llm_templates.py` & `autotransformers-0.0.8/src/autotransformers/llm_templates.py`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/metrics.py` & `autotransformers-0.0.8/src/autotransformers/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,16 +67,16 @@
     preds, labels = pred.predictions, pred.label_ids
     preds = torch.sigmoid(torch.from_numpy(preds)).numpy()
     thresholds = np.arange(0.1, 0.9, 0.1)
     best_metrics, best_metric, best_threshold = {}, 0, None
 
     for thres in thresholds:
         preds = preds >= thres
-        preds = preds.astype(np.int)
-        labels = labels.astype(np.int)
+        preds = preds.astype(int)
+        labels = labels.astype(int)
         class_report = classification_report(
             labels,
             preds,
             output_dict=True,
         )
         metrics = class_report["macro avg"]
         f1 = metrics["f1-score"]
```

### Comparing `autotransformers-0.0.7/src/autotransformers/metrics_plotter.py` & `autotransformers-0.0.8/src/autotransformers/metrics_plotter.py`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/model_config.py` & `autotransformers-0.0.8/src/autotransformers/model_config.py`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/results_getter.py` & `autotransformers-0.0.8/src/autotransformers/results_getter.py`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/tokenization_functions.py` & `autotransformers-0.0.8/src/autotransformers/tokenization_functions.py`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/src/autotransformers/utils.py` & `autotransformers-0.0.8/src/autotransformers/utils.py`

 * *Files identical despite different names*

### Comparing `autotransformers-0.0.7/PKG-INFO` & `autotransformers-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotransformers
-Version: 0.0.7
+Version: 0.0.8
 Summary: a Python package for automatic training and benchmarking of Language Models.
 Home-page: https://lenguajenatural.ai
 License: CC BY-NC-SA 4.0
 Keywords: large-language-models,language-models,natural-language-processing,nlp,transformers,hyperparameter-tuning,automatic-training
 Author: LenguajeNatural.AI
 Author-email: avaca@lenguajenatural.ai
 Requires-Python: >=3.9.13,<4.0.0
@@ -450,7 +450,19 @@
     dataset_configs = [data_config]
 )
 
 autotrainer()
 ```
 
 In this way, we are using the pipeline to internally augment data before training, therefore we will increment the amount of training data, without modifying the validation and test subsets.
+
+## Citation
+
+```
+@misc{vaca2024autotransformers,
+    author = {Alejandro Vaca Serrano},
+    title = {AutoTransformers: A Library for Automatic Training and Benchmarking of Transformer Models},
+    year = {2024},
+    howpublished = {\url{https://github.com/lenguajenatural-ai/autotransformers}},
+}
+```
+
```

